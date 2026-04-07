## Decomposition-Based Reformulation of Nonseparable Quadratic Expressions in Convex MINLP

This repository contains all test instances used in the numerical experiments reported in XXXXXXX. These include selected problems from [MINLPLib](https://www.minlplib.org/instances.html) and newly generated instances to test the decomposition-based reformulations. In addition, the repository includes all data that support the findings.

### Repository Structure
- [Generated Instances](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances) - Problem instances generated for this study, grouped by model variant.
  - [CCPOP](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances/CCPOP) - Cardinality-Constrained Portfolio Optimization Problem
  - [CCPOPwTCaD](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances/CCPOPwTCaD) - Cardinality-Constrained Portfolio Optimization with Transaction Costs and Diversification
  - [CCPOPwTCaRL](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances/CCPOPwTCaRL) - Cardinality-Constrained Portfolio Optimization with Transaction Costs and Risk Limit
  - [RPOPwCaTC](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances/RPOPwCaTC) - Robust Portfolio Optimization with Cardinality and Transaction Costs
  - [CCPOPwTCRTEaD](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances/CCPOPwTCRTEaD) - Cardinality-Constrained Portfolio Optimization with Risk, Tracking Error, Diversification, and Transaction Costs
  - [SaCCDPOP](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances/SaCCDPOP) - Sector-Constrained Diversified Portfolio Optimization Problem
  - [MPCCPOP](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances/MPCCPOP) - Multi-Period Portfolio Optimization Problem
  - [MPCCPOP_crypto](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/Generated%20Instances/MPCCPOP_crypto) - Multi-Period Crypto Portfolio Optimization Problem
- [MINLPLib Instances](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Test%20Instances/MINLPLib%20Instances) - Selected problems from MINLPLib
- [Results](https://github.com/AAU-IT/quad-decomp-convex-minlp/tree/main/Results) - Paver reports and trace files

### Test Instances

#### Generated Instances
There are **eight different types of portfolio optimization problems**. 
Each problem type has its own folder. Inside each folder you will find:
- **a Jupyter notebook ('.ipynb'):**
  Explains how the problems were generated using **GAMSPy**.
  The mathematical model of the problem.
  Solver setup and code for generating the instances.
- **a GAMS folder:**
  Contains the '.gms' files used in the tests. 

The table below summarizes all new instances:

| Name                      | Type   | C      | #Vars  | #BinVars | #IntVars | #Cons  |
|---------------------------|--------|--------|--------|----------|----------|--------|
| CCPOP5_20                 | MBQP   | Convex | 40     | 20       | 0        | 22     |
| CCPOP5_50                 | MBQP   | Convex | 100    | 50       | 0        | 52     |
| CCPOP5_100                | MBQP   | Convex | 200    | 100      | 0        | 102    |
| CCPOP5_186                | MBQP   | Convex | 372    | 186      | 0        | 188    |
| CCPOP5_219                | MBQP   | Convex | 438    | 219      | 0        | 221    |
| CCPOP5_300                | MBQP   | Convex | 600    | 300      | 0        | 302    |
| CCPOPwTCaD5_20            | MBQCQP | Convex | 40     | 20       | 0        | 23     |
| CCPOPwTCaD5_50            | MBQCQP | Convex | 100    | 50       | 0        | 53     |
| CCPOPwTCaD5_100           | MBQCQP | Convex | 200    | 100      | 0        | 103    |
| CCPOPwTCaD5_300           | MBQCQP | Convex | 600    | 300      | 0        | 303    |
| CCPOPwTCaRL5_20           | MBQCQP | Convex | 40     | 20       | 0        | 23     |
| CCPOPwTCaRL5_50           | MBQCQP | Convex | 100    | 50       | 0        | 53     |
| CCPOPwTCaRL5_165          | MBQCQP | Convex | 330    | 165      | 0        | 168    |
| CCPOPwTCaRL5_308          | MBQCQP | Convex | 616    | 308      | 0        | 311    |
| CCPOPwTCaRL5_538          | MBQCQP | Convex | 1076   | 538      | 0        | 541    |
| RPOPwCaTC5_20             | MBQCQP | Convex | 42     | 20       | 0        | 26     |
| RPOPwCaTC5_50             | MBQCQP | Convex | 102    | 50       | 0        | 56     |
| RPOPwCaTC5_100            | MBQCQP | Convex | 202    | 100      | 0        | 106    |
| RPOPwCaTC5_319            | MBQCQP | Convex | 640    | 319      | 0        | 325    |
| CCPOPwTCRTEaD5_20         | MBQCQP | Convex | 40     | 20       | 0        | 25     |
| CCPOPwTCRTEaD5_50         | MBQCQP | Convex | 100    | 50       | 0        | 55     |
| SaCCDPOP5_3_17            | MBNLP  | Convex | 50     | 25       | 0        | 53     |
| SaCCDPOP5_3_61            | MBNLP  | Convex | 132    | 66       | 0        | 135    |
| SaCCDPOP5_3_115           | MBNLP  | Convex | 240    | 120      | 0        | 243    |
| SaCCDPOP5_3_326           | MBNLP  | Convex | 662    | 331      | 0        | 665    |
| MPCCPOP12_10              | MBQP   | Convex | 2160   | 720      | 0        | 1585   |
| MPCCPOP12_20              | MBQP   | Convex | 4320   | 1440     | 0        | 3025   |
| MPCCPOP12_30              | MBQP   | Convex | 6480   | 2160     | 0        | 4465   |
| MPCCPOP12_50              | MBQP   | Convex | 10800  | 3600     | 0        | 7345   |
| MPCCPOP_crypto8_1mo_1d    | MBQP   | Convex | 481    | 240      | 0        | 541    |
| MPCCPOP_crypto8_1mo_5d    | MBQP   | Convex | 97     | 48       | 0        | 109    |
| MPCCPOP_crypto8_6d_30m    | MBQP   | Convex | 4081   | 2040     | 0        | 4591   |
| MPCCPOP_crypto8_30d_90m   | MBQP   | Convex | 7505   | 3752     | 0        | 8443   |

#### MINLPLib Instances
The table below summarizes all instances from MINLPLib:

| Name                      | Type   | C      | #Vars  | #BinVars | #IntVars | #Cons  |
|---------------------------|--------|--------|--------|----------|----------|--------|
| alan                      | MBQP   | Convex | 8      | 4        | 0        | 7      |
| ball_mk4_05               | IQCP   | Convex | 10     | 0        | 10       | 20     |
| ball_mk4_10               | IQCP   | Convex | 20     | 0        | 20       | 40     |
| ball_mk4_15               | IQCP   | Convex | 30     | 0        | 30       | 60     |
| color_lab2_4x0            | BQP    | Convex | 300    | 300      | 0        | 61     |
| color_lab6b_4x20          | BQP    | Convex | 235    | 235      | 0        | 48     |
| du-opt                    | MIQP   | Convex | 20     | 0        | 13       | 46     |
| du-opt5                   | MIQP   | Convex | 20     | 0        | 13       | 46     |
| fac3                      | MBQP   | Convex | 66     | 12       | 0        | 33     |
| meanvar-orl400_05_e_8     | MBQP   | Convex | 1600   | 400      | 0        | 1603   |
| meanvarx                  | MBQP   | Convex | 35     | 14       | 0        | 44     |
| nvs10                     | IQCQP  | Convex | 2      | 0        | 2        | 2      |
| nvs11                     | IQCQP  | Convex | 3      | 0        | 3        | 3      |
| nvs12                     | IQCQP  | Convex | 4      | 0        | 4        | 4      |
| nvs15                     | IQP    | Convex | 3      | 0        | 3        | 1      |
| pedigree_ex1058           | MBQCP  | Convex | 1059   | 999      | 0        | 867    |
| pedigree_ex485            | MBQCP  | Convex | 485    | 426      | 0        | 296    |
| pedigree_ex485_2          | MBQCP  | Convex | 485    | 426      | 0        | 296    |
| pedigree_sim2000          | MBQCP  | Convex | 2000   | 1000     | 0        | 794    |
| pedigree_sim400           | MBQCP  | Convex | 400    | 150      | 0        | 101    |
| pedigree_sp_top4_250      | MBQCP  | Convex | 845    | 713      | 0        | 416    |
| pedigree_sp_top4_300      | MBQCP  | Convex | 605    | 473      | 0        | 246    |
| pedigree_sp_top4_350tr    | MBQCP  | Convex | 269    | 262      | 0        | 147    |
| pedigree_sp_top5_200      | MBQCP  | Convex | 1390   | 1258     | 0        | 873    |
| pedigree_sp_top5_250      | MBQCP  | Convex | 967    | 835      | 0        | 538    |
| watercontamination0202r   | MBQP   | Convex | 195    | 7        | 0        | 283    |
| watercontamination0303r   | MBQP   | Convex | 384    | 14       | 0        | 556    |


**This repository is licensed under the MIT License.** 