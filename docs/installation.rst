Installation
============

Install with Pip
----------------

.. code-block:: bash 

	pip install picaso


Install with Git
----------------

.. code-block:: bash 

	git clone https://github.com/natashabatalha/picaso.git
	cd picaso
	python setup.py install 

Download and Link Reference Documentation
-----------------------------------------

1) If you did not download the github repository, make sure you pull the `Reference Folder <https://github.com/natashabatalha/picaso/tree/master/reference>`_.  

2) Now you can create an environment variable:


.. code-block:: bash

	vi ~/.bash_profle

Add add this line:

.. code-block:: bash

	export picaso_refdata="/path/to/picaso/reference/"

Should look something like this 

.. code-block:: bash

	cd /path/to/picaso/reference/data
	ls
	base_cases	config.json	opacities

Download and Link Pysynphot Stellar Data
----------------------------------------

In order to get stellar spectra you will have to download the stellar spectra here from PySynphot: 

1) Download the `stellar spectra from here <https://pysynphot.readthedocs.io/en/latest/appendixa.html>`_. The Defulat for `PICASO` is Castelli-Kurucz Atlas: `ck04models <https://archive.stsci.edu/hlsps/reference-atlases/cdbs/grid/ck04models/>`_. 

2) Create environment variable

.. code-block:: bash

	vi ~/.bash_profle

Add add this line:

.. code-block:: bash

	export PYSYN_CDBS="/path/to/data/files/grp/hst/cdbs"

Should look something like this 

.. code-block:: bash

	cd /path/to/data/files/grp/hst/cdbs
	ls
	grid

Where `grid` contains whatever `pysynphot` data files you have downloaded (e.g. a folder called `ck04models`). 
