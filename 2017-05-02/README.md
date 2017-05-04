Daily log: 2017-05-02

**I. Finding source of background variation for 628 nm laser excitation

II. Fine alignment

III. determination of R and G LCOS rotations

IV. sm measurements!!**



-----------------------------------------------------------------------

**I. Finding source of background variation for 628 nm laser excitation**

- variation over long time scales was observed with R excitation
  (smFRET mixture with 7d and 22d, measured by Maya on 2017-04-30)
- in order to try to understand this we calculated the brightness
  ratio of ATTO647N and ATTO550 by taking the product of the acceptor
  absorption cross-section at ex wavelength 628nm and the quantum yield
  of the acceptor and dividing by the donor absorption
  cross-section multiplied by the donor quantum yield. See 'dyes' folder
  for notebooks.

**CONCLUSION**

- ATTO647N is brighter than ATTO550, **however** this result conflicts
  with our observation that the R laser fluctuates and has very high
  background at powers above 100mW.

**II. Fine alignment**

- R SPAD is misaligned --> Antonio updated R conf with fit results from
  multicounter scans because we **cannot more the R SPAD after aligned it to the
  G laser**
- Instead of moving R SPAD to fitted position, adjust LCOS center position in GUI
  to conf to match location of fitted R spots



**III. determination of R and G LCOS rotations**

- Rotation for G and R LCOS was configurations were determined with
  'alignment summary' notebook results. We selected an average rotation value.
- R_rot was changed from 0.3 degrees to -1.3 degrees
- G_rot was changed from 0 degrees to 1.31 degrees
- NOTE: R_rot is reversed wrt G_rot because R LCOS is mirrored

**CONCLUSION**

- R LCOS rot = -1.30 (conf3_R)
- G LCOS rot = 1.31 (conf2_G)

**IV. sm measurements!!**

- sm measurements of 12d dsDNA sample at different powers
- signal from 532nm laser is much more intense than signal from the 628nm laser,
  even when both laser powers are set to 100mW and power is maximized with
  the half wave plate
- smFRET measurements look good! Still need to determine source of high, fluctuating
  R background
- Test measurements are saved in smdata folder:

1) R laser only

2) R laser only, AOM on and alternation OFF - changed sample, same dilution tube

3) R and G lasers, AOM on and alternation OFF - same gasket from 2)
