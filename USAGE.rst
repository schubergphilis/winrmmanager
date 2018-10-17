=====
Usage
=====


To develop on winrmmanager:

.. code-block:: bash

    # The following commands require pipenv as a dependency

    # To lint the project
    _CI/scripts/lint.py

    # To execute the testing
    _CI/scripts/test.py

    # To create a graph of the package and dependency tree
    _CI/scripts/graph.py

    # To build a package of the project under the directory "dist/"
    _CI/scripts/build.py

    # To see the package version
    _CI/scipts/tag.py

    # To bump semantic versioning [major|minor|patch]
    _CI/scipts/tag --major|--minor|--patch

    # To upload the project to a pypi repo if user and password is properly provided
    _CI/scripts/upload.py

    # To build the documentation of the project
    _CI/scripts/document.py



To use winrmmanager in a project:

.. code-block:: python

    from winrmmanager import Winrmmanager
    winrmmanager = Winrmmanager(host,
                                username,
                                password)
    valid_session = winrmmanager.get_session()
