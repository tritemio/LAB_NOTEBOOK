Ordering donor emission filter from Semrock -
in order to determine correct filter Antonio wrote a notebook with
spectra, dichroics, and filters. The best filters options are
580/60nm
582/75nm

Antonio added multiple components to labview:
- metadata_48spot vi for storing single YAML files with experimental
detail on the computer
- metadata will be sent to the server computer
where YAML metadata files will be archieved (4 Tb hard drive)
- measurement data will be sent to the server computer where .dat
files will be converted to Hdf5 files and archived
** in this way, there will be two copies of .dat files,
one on each computer.

To do:
- Emission, excitation and optics notebook
- measure dsDNA sample measured 2017-04-04 on usALEX set up as
simple control
- take DCR data
- align red laser to pattern better (?)
- document and begin writing paper/proposal
