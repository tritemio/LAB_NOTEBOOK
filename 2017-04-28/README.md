DATA IS GOOD FOR MANUSCRIPT

**I. File organization
II. Adjusting LCOS patterns for better pattern matching
III. Test addition of slit for improved signal**




----------------------------------------------------------
**I. File organization**

Files were reorganized such that notebooks can be run from
any computer via relative path. Absolute paths require that the
user update the path before running the notebook, hindering the
analysis/data retrieval process.

- Data folder now contains instrument subfolders
    * e.g. manta=48-spot, 8-spot, usALEX, etc.
- instrument subfolders each contain subfolders, e.g.
    * Alignment - dated data folders, notebooks for
      alignment analyses
    * DCR - dated data folders
    * Notebook - all notebooks related to instrument of interest

**II. Adjusting LCOS patterns for better overlap**

NOTE: Images of each configuration were collected and analyzed with
      'LCOS pattern fitting' notebook.

- conf1_G: image taken from old (unknown date) settings

- conf2_G: image taken with conf1 from 2017-04-25

- conf3_G: 11x11, adjusted G LCOS center and then matched R LCOS
           center to new conf

- conf4_G: moved both LCOSs up 2 pixels

- conf5_G: moved G LCOS to the right on the camera

.
.
.

- conf9_G: FIXING G LCOS CONF TO **conf9**

- scanning G SPAD and fine aligning to new center

- G LCOS position is good, but when we look at both patterns
  overlayed they are not aligned... We are now running the notebook
  for the R pattern. Optical axis looks (rotation heat map shows pattern overlay with respect to the optical axis) good but the intensity is low and to the right in
  the notebook (transposed) ---> up and to the right on the camera.


-----------------------------------------------------------

- conf1_R: image taken from old (unknown date) settings

- conf2_R: image taken with conf16 from 2017-04-25

- conf3_R: 11x11, adjusted G LCOS center and then matched R LCOS
           center to new conf

- conf4_R: moved both LCOSs up 2 pixels

- conf5_R: moved R LCOS to the right on the camera (so more negative in x of
           LCOS and down in the notebook...)

.
.
.

- conf10_R:

- Realign far and close mirrors of R beam path with conf9_R

- Added rotation to R LCOS - cw rot input in LCOS GUI = ccw rot in camera

- conf14_R: FIXING R LCOS CONF TO **conf14**

**CONCLUSION**:

- GLCOS: conf9; new center (2,-67)
- RLCOS: conf14; new center (10.21, 19.71)
- angle of R LCOS = angle of G LCOS + 0.25 degrees
- Accuracy in x,y < 0.03 LCOS pixels - this method may be better than scanning!!

**III. Test addition of slit for improved signal**

NOTE: Images of each configuration were collected and analyzed with
'Slit no slit comparison' notebook

- filenames end with slit '_ slit'
- other files without 'slit' were without slits

**IV. Scanning R SPAD**

- scans for the day are saved in two .txt files in alignment folder

**Alignment protocol - notes**

Use camera with 647LP em filter to center G LCOS
  - use an odd, square pattern to easily locate center position, e.g. 11x11
