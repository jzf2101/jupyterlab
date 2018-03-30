.. _installation:

Installation
------------

JupyterLab can be installed using ``conda``, ``pip``, or ``pipenv``.
To develop JupyterLab, see our :ref:`developer instructions <dev_install>`.

conda
~~~~~

If you use ``conda``, you can install it with:

.. code:: bash

    conda install -c conda-forge jupyterlab

pip
~~~

If you use ``pip``, you can install it with:

.. code:: bash

    pip install jupyterlab


If installing using ``pip install --user``, you must add the user-level
``bin`` directory to your ``PATH`` environment variable in order to launch
``jupyter lab``.

pipenv
~~~~~~

If you use ``pipenv``, you can install it as:

.. code:: bash

    pipenv install jupyterlab
     pipenv shell

or from a git checkout:

.. code:: bash

    pipenv install git+git://github.com/jupyterlab/jupyterlab.git#egg=jupyterlab
     pipenv shell

When using ``pipenv``, in order to launch ``jupyter lab``, you must activate the project's virtualenv.
For example, in the directory where ``pipenv``'s ``Pipfile`` and ``Pipfile.lock`` live (i.e., where you ran the above commands):

.. code:: bash

    pipenv shell
     jupyter lab

Installing with Previous Versions of Notebook
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If you are using a version of Jupyter Notebook earlier than 5.3, then you must also run the following command to enable the JupyterLab
server extension:

.. code:: bash

    pipenv install jupyterlab
     pipenv shell

or from a git checkout:

.. code:: bash

    pipenv install git+git://github.com/jupyterlab/jupyterlab.git#egg=jupyterlab
     pipenv shell

When using ``pipenv``, in order to launch ``jupyter lab``, you must activate the project's virtualenv.
For example, in the directory where ``pipenv``'s ``Pipfile`` and ``Pipfile.lock`` live (i.e., where you ran the above commands):

.. code:: bash

    pipenv shell
     jupyter lab

.. _prereqs:

Prerequisites
~~~~~~~~~~~~~

JupyterLab requires the Jupyter Notebook version 4.3 or later. To check
the version of the ``notebook`` package that you have installed:

.. code:: bash

    jupyter notebook --version

    JupyterLab requires Jupyter Notebook version 4.3 or later.

If you use ``conda``, you can install notebook using:

.. code:: bash
    conda install -c conda-forge notebook

or with ``pip``:

.. code:: bash

    pip install notebook

You may also want to install `nb_conda_kernels` to have a kernel option for different [conda environments](http://conda.pydata.org/docs/using/envs.html).
With ``conda``:

.. code:: bash

    conda install -c conda-forge nb_conda_kernels
