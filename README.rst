stGP tutorial
=============

Source code for building the tutorial website of ``stGP``.

The website is configured for Read the Docs at:

https://stgp-tutorial.readthedocs.io/

The tutorial notebooks cover:

* Human aging DLPFC MERFISH analyses.
* Mouse aging brain MERFISH microglia analyses.
* Mouse injured kidney Xenium analyses.

Build the documentation locally with:

.. code-block:: bash

   python -m pip install -r docs/requirements.txt
   sphinx-build -b html docs/source docs/_build/html

Notebook execution is disabled during documentation builds so the website can
render without large local datasets.
