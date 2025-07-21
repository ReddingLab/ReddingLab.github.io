---
layout: protocol
title: HP1 purification 
category: protein 
# author: Sy 
---

### Buffers


| Lysis Buffer   | Final Concentration     |
| ---------------------:| -----------------------:|
| Tris-HCl, pH7.5       | 20mM                    |
| NaCl                  | 300mM                   |
| Imidazole             | 7.5mM                   |
| Gycerol               | 10%                     |
| protease inhibitors          | 1 tablet/50mL           |

| Wash Buffer   | Final Concentration     |
| ---------------------:| -----------------------:|
| Tris-HCl, pH 8        | 20mM                    |
| NaCl                  | 150mM                   |
| Imidazole             | 7.5mM                   |

| Elution Buffer   | Final Concentration     |
| ---------------------:| -----------------------:|
| Tris-HCl, pH 8        | 20mM                    |
| NaCl                  | 150mM                   |
| Imidazole             | 400mM                   |

| TEV cleavage Buffer   | Final Concentration     |
| ---------------------:| -----------------------:|
| Tris-HCl, pH 8        | 20mM                    |
| NaCl                  | 100mM                   |
| DTT                   | 3mM                     |

| Buffer A   | Final Concentration     |
| ---------------------:| -----------------------:|
| Tris-HCl, pH 8        | 20mM                    |
| KCl                  | 100mM                   |
| DTT                   | 1mM                     |

| Buffer B | Final Concentration     |
| ---------------------:| -----------------------:|
| Tris-HCl, pH 8        | 20mM                    |
| KCl                  | 800mM                   |
| DTT                   | 1mM                     |

| SEC Buffer   | Final Concentration     |
| ---------------------:| -----------------------:|
| Tris-HCl, pH 8        | 20mM                    |
| KCl                  | 200mM                   |
| DTT                   | 1mM                     |
| Gycerol               | 10%                     |



### Protocol

Step 1: Transform Rosetta competent cells with HP1 vector

Step 2: Grow overnight culture of 50mL from single colony

Step 3: Large culture growth
* Grow cells in 2L of 2xLB at 37C to an OD600 of 1.0–1.4. Induce expression induced by adding 0.3 mM IPTG and grow cells for an additional 3 hr at 37C.
* Pellet cells at 5000xg for 30 min. (pellets can be frozen and stored at -80C)

Step 4: His-tag purification
*	For next day
    *   Equilibrate a Q column in buffer A
    *   Equilibrate S-75 column in SEC buffer
*   Resuspend cell pellets in 30 mL Lysis Buffer 
*	Lyse cells by sonication (~30% power 15s on 1m off for 10 cycles)
*	Clarify the lysate by centrifugation at 30,000xg for 30 min. 
*	Next add the supernatant to 1 mL/Liter culture of Talon cobalt resin and incubate with rotation for 1 hr at 4°C. 
*	Then add the resin-lysate mixture to a gravity column and wash with 100mL lysis buffer without protease inhibitors.
*	Elute the protein in 10mL of elution buffer 
*	Then combine eluted protein with one tube of purified super-TEV protease and dialyze overnight into TEV cleavage buffer at 4°C. 


Step 5: Anion exchange
*   Recover the protein from dialysis and load onto equilibrated Q column. 
*	Wash with buffer A until UV signal is at baseline on FPLC.
*	Then elute HP1 by a salt gradient. Switch from 100% buffer A to 100% buffer B over ~16 column volumes. 

Step 6: Size exclusion
*	Concentrate pooled protein fractions from the anion exchange column and concentrate in a spin concentrator to ~500 μL.
*	Load sample onto a Superdex-75 Increase column with SEC buffer
*	Pool protein containing fractions and concentrate to ~500uL in a 10K spin concentrator.
*	Finally, flash freeze aliquots in liquid nitrogen and store at −80°C


