Usage
=====

The tutorials are organized by biological system:

* Human aging DLPFC MERFISH examples for excitatory neurons and
  oligodendrocytes.
* Mouse aging brain MERFISH examples for microglia and downstream analyses.
* Mouse injured kidney Xenium examples for injured proximal tubule and immune
  cell analyses.

Running notebooks
-----------------

Open the repository root as the working directory, then launch Jupyter:

.. code-block:: bash

   jupyter lab

Most notebooks expect processed ``.h5ad`` files and saved ``stGP`` result
objects under local ``data/``, ``Results/``, ``Figure/``, or ``Figures/``
directories. These large generated files are intentionally not part of the
documentation source.

Website rendering
-----------------

Read the Docs uses ``docs/source/conf.py`` and ``.readthedocs.yaml`` to build
the website. Notebook execution is disabled during documentation builds:

.. code-block:: python

   nbsphinx_execute = "never"

This makes the website a stable rendered tutorial even when the analysis data
are stored separately.
