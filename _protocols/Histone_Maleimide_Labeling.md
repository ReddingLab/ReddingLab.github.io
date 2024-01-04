---
layout: protocol
title: Histone Maleimide Labeling 
catagory: reagent 
pdf: /static/img/protocols/Histone_Maleimide_Labeling.pdf
# author: Liv Jensen
---


Materials:

-   Atto488 maleimide (Sigma, 28562)

-   5ml HiTrap desalting column (GE, 29-0486-84)

-   TCEP

-   Lyophilized histone

Labeling Buffer:


|                       | 50 mL         | Final Concentration  |
| -------------         |:-------------:| -----:|
| 1M Tris, pH7.0        | 1mL           | 20mM    |
| GuCl (MW: 95.5g/mol)  | 33.4g         |   7M |
| 0.25M EDTA            | 1mL           |   5mM |

 

Procedure:

1.  Bring up TCEP to 0.5M, adjust pH to 7.5.

2.  Bring up histone in labeling buffer to 0.5mM final concentration.

 * for H2A 120C, 3.6 mg of histone goes into 516uL labeling buffer
 * epsilon = 0.317, MW = 14081g/mol

1.  Add TCEP to histone to final concentration of 0.7mM.

2.  Incubate at RT for 2 hrs.

3.  Dissolve Atto488 maleimide in DMSO to 100mM, vortex and spin down to
    completely dissolve. Wrap tube in foil and store at -20C.

* for 1mg Atto488, dissolve in 9.37uL DMSO
* Atto488 maleimide MW: 1067g/mol

1.  Add Atto488 maleimide to histone:

* for 5ml desalting column, optimal load volume is 100uL-1.5mL; 200uL reaction volumes work well.
* alternative desalting method is to dialyze labeling reaction into labeling buffer in which case you don't need to worry about reaction volumes; dialysis desalting method seems to work well for Atto488 and Atto565


|                       | 50 mL         | Final Concentration  |
| -------------         |:-------------:| -----:|
| 100mM Atto488         | 1.2uL        |   0.6mM |
| 0.5mM histone         | 40uL         |   0.1mM |
| Water                 | 158.8uL      |    |



Incubate 3 hr at RT, then O/N at 4C

1.  Equilibrate HiTrap desalting column with labeling buffer at 4C.

    a.  Load sample at 1ml/min, collect 200uL fractions.

    b.  Observe 2 peaks, 1^st^ narrow and 2^nd^ broad

2.  Run SDS-PAGE and visualize with Typhoon imager in Atto488 channel,
    then coomassie stain.

    a.  1st peak corresponds to protein (labeled and unlabeled elute
        together)

    b.  2nd peak corresponds to free dye

3.  Assess labeling efficiency by NanoDrop (delta between molarity
    calculated from Atto488 absorbance and molarity calculated from
    histone absorbance)


