Blaauw Observatory Knowledgebase
================================

This is the Github repository for information regarding the Blaauw Observatory.
The documentation is hosted at `readthedocs`_.


.. _readthedocs: https://blaauwobserverknowledgebase.readthedocs.io/en/latest/

Here are some useful links if you want to know more about how the project is set up:

* `reStructuredText (RST) Primer <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_
* `Sphinx + RST + Readthedocs Tutorial <https://sphinx-tutorial.readthedocs.io/>`_
* `Readthedocs Tutorial <https://docs.readthedocs.io/en/stable/tutorial/>`_


Making changes
==============

You can make changes by editing files in Github directly, but then you will only be able
to see and test your changes after Readthedocs compiles them. So this mostly
works for small changes.

A better alternative is to set up the project locally (assuming you have a
Linux system and git installed) and generate the documentation yourself:

1. Start wil cloning the repository

    .. code-block:: bash

       git clone https://github.com/PracticalAstronomyCrew/knowledgebase.git
       # or with SSH set up (better!)
       git clone git@github.com:PracticalAstronomyCrew/knowledgebase.git

       # Then move into the cloned repository
       cd knowledgebase

2. Create a virtual environment, activate it and install the Sphinx dependencies

    .. code-block:: bash

       # Creates a subdirectory .venv, change the name if you want
       python3 -m venv .venv  

       source .venv/bin/activate   # Activates the virtual environment

       # Installs the dependencies for compiling the documentation
       pip install -r ./docs/requirements.txt  

3. Build the html pages of the local documentation:

    .. code-block:: bash

        # Run 'make html' in the ./docs subdirectory
        make html -C docs

4. If this was successful the HTML pages can now be found in the directory:
   ``docs/build/html``. Open them (for instance with firefox) like this:

    .. code-block:: bash

        firefox ./docs/build/html/index.html

Now you should be ready to make changes to the knowledgebase. If you are ready
to see your changes locally, you can rebuild (step 3.) and reopen the pages
(step 4.).

Finally, if you are completely done and satisfied with your changes (make sure
it builds successfully!) you can ``add``, ``commit`` and ``push`` your changes.
