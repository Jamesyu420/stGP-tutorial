Installation
============

To install the released ``stgp`` package from PyPI into your current Python
environment:

.. code-block:: shell

   pip install stgp

To reproduce the notebooks from the GitHub repository, you can also install the
stGP environment from GitHub:

.. code-block:: bash

   git clone https://github.com/YangLabHKUST/stGP.git
   cd stGP
   conda env create -f stGP.yml
   conda activate stGP
   pip install -e .

Normally the installation time will be less than twenty minutes. The package has
been tested on Linux (Ubuntu 22.04.5 LTS).

Build the tutorial documentation locally
----------------------------------------

Clone the tutorial repository:

.. code-block:: bash

   git clone git@github.com:Jamesyu420/stGP-tutorial.git
   cd stGP-tutorial

For documentation builds, install the Sphinx requirements:

.. code-block:: bash

   python -m pip install -r docs/requirements.txt

Then build the documentation:

.. code-block:: bash

   sphinx-build -b html docs/source docs/_build/html

The documentation build renders notebooks without executing them, so the build
does not require the large input datasets.
