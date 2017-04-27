**ALIGNMENT**     2017-04-26

No slit

**I. CENTERING 628nm BEAM**

- Aligning R beam intensity wrt to R SPAD:

Real1: changed angle with far LCOS mirror
Real2: translated beam 'down' by adjusting far mirror then near mirror
Real3: translated beam 'down' by adjusting far mirror then near mirror
Real4: translated beam 'down' by adjusting far mirror then near mirror
Real5: translated beam 'down' by adjusting far mirror then near mirror
Real6: translated beam horizontally with near mirror
       to fix rotation of Gaussian fit in 2D

**Note**: This method of alignment is not sensitive to changes in pitch

**II. Determining R LCOS configuration**

- Configurations were analyzed with 'LCOS pattern fitting' notebook.
  Resulting configurations were tested with notebook results of previous conf.

Conf1: (R,G) from 2017-04-25
Conf2: (R) after Real(?)
Conf3: (R) after Real(?)
Conf4: (R) after Real6
Conf5: (R) after 0.5 degree rotation
Conf6: (R) after 0.2 degree rotation
Conf7: (R) after adjusting center H,V and pitch x,y
Conf8: (R) after adjusting center H
Conf9: (R) from results of conf8 analysis
Conf10: (R) from results of conf9 analysis
Conf11: (R) from results of conf10 analysis

**NOTE**: Antonio found a bug in the notebook i.e. we plot the **transpose**
of the image to save space in the the notebook. The transpose is a rotation
plus a mirroring. so (x,y) coordinates refer to notebook:

Conf12: (R) fitted from conf1, img8
Conf13: (R) testing directionality of center H,V on LCOS by changing
        sign in notebook and comparing to reverse sign of previous notebook.

*Conf1*: (R) conf1, img 9  
Conf14: (R) TESTING code: conf1 adjusted center H by +2 LCOS units
Conf15: (R) fitted from conf1, images 9 and 10
Conf16: (R) fitted from conf15, images 1, 2, and 3

Antonio noticed variability in output parameters after many iterations.
He anticipates that we can fit with up to 0.1 pixel accuracy.
We will compare accuracy across methods to see which is best and what
information we can extract from each method.

HYPOTHESIS: we expect scans to be more accurate than this camera method

- X in notebook maps to V of LCOS
- Y in notebook maps to H of LCOS
- 'LCOS pattern fitting' notebook was corrected accordingly.

Because of this we are repeating this procedure, **with the correct axes**,
unlike before... For this we begin with conf1 and analyze images of R LCOS
in **axes corrected** 'LCOS pattern fitting' notebook.

**III. conf15 variability**

Statistics of last three images of conf15 were collected and analyzed.

CONCLUSIONS:

- pitch accuracy ~ 0.05 LCOS units
- center position accuracy < ~ 0.1 - 0.02 LCOS units

**Use conf15 for the R LCOS** 
