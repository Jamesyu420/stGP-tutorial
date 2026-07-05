Installation
============

This tutorial repository focuses on analysis notebooks. The notebooks assume a
Python environment with common spatial transcriptomics and scientific computing
packages installed.

Clone the tutorial repository
-----------------------------

.. code-block:: bash

   git clone git@github.com:Jamesyu420/stGP-tutorial.git
   cd stGP-tutorial

Create an analysis environment
------------------------------

Use the environment that contains your local ``stGP`` installation and the
packages used by the notebooks, including ``scanpy``, ``numpy``, ``pandas``,
``scipy``, ``matplotlib``, and ``ipykernel``.

For documentation builds only, install the Sphinx requirements:

.. code-block:: bash

   python -m pip install -r docs/requirements.txt

Build the documentation locally
-------------------------------

.. code-block:: bash

   sphinx-build -b html docs/source docs/_build/html

The documentation build renders notebooks without executing them, so the build
does not require the large input datasets.
