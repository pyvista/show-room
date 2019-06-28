You can get the data from the
[SEG-website](https://wiki.seg.org/wiki/SEG/EAGE_Salt_and_Overthrust_Models)
or via the
[direct link](https://s3.amazonaws.com/open.source.geoscience/open_data/seg_eage_models_cd/Salt_Model_3D.tar.gz).
The zip-file is 513.1 MB big. Unzip the archive and proceed.

Copy the `'Salt_Model_3D/3-D_Salt_Model/SURFACES/'` folder to the `'./data/'`
directory in this repository

place the file `Salt_Model_3D/3-D_Salt_Model/VEL_GRIDS/SALTF.ZIP` (20.0 MB)
into `./data/` (or adjust the path in the following cell).

The following cell loads the resistivity model `res-model.lzma` (~14 MB), if
it already exists in `./data/`, or alternatively loads the velocity model
`Saltf@@`, carries out the velocity-to-resistivity transform, and stores the
resistivity model.
