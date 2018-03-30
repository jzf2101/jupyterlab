.. _starting:

Starting JupyterLab
-------------------

Start JupyterLab using:

.. code:: bash

    jupyter lab

JupyterLab will open automatically in your browser. You may also access
JupyterLab by entering the notebook server's URL (usually
``http://localhost:8888``) into the browser. You can also open the
classic Notebook from JupyterLab by selecting "Launch Classic Notebook"
from the JupyterLab Help menu.

Because JupyterLab is a server extension of the classic Jupyter Notebook
server, you can also use JupyterLab by starting the classic Jupyter
Noteboook (``jupyter notebook``) and visiting the ``/lab`` URL (usually
``http://localhost:8888/lab``) rather than the default ``/tree`` URL.
Conversely, to go to the classic Notebook from JupyterLab, you can
change the URL from ``/lab`` to ``/tree``.

Supported browsers
~~~~~~~~~~~~~~~~~~

The latest versions of the following browsers are currently known to work:

-  Firefox
-  Chrome
-  Safari

Earlier browser versions may also work, but come with no guarantees.

JupyterLab uses CSS Variables for styling, which is one reason for the
minimum versions listed above.  IE 11+ or Edge 14 do not support
CSS Variables, and are not directly supported at this time.
A tool like `postcss <http://postcss.org/>`__ can be used to convert the CSS files in the
``jupyterlab/build`` directory manually if desired.

Security
~~~~~~~~

JupyterLab has the same security model as the classic Jupyter Notebook;
for more information see the `security
section <https://jupyter-notebook.readthedocs.io/en/stable/security.html>`__
of the classic Notebook's documentation.
