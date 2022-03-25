# Decision-Tree-SAS-Miner

**Dataset:** StudentPerformance.csv

**Steps:**
1. Create Diagram
2. Drag File import from sample and Import Student Performance
3. Edit Variables (i.e, set Gender as Target)
4. Drag Data Partition node from sample tab
5. Change Dataset splitting ratio: training 40, validation 40, test 20
6. Drag Decision Tree node from model tab
7. Run the Decision Tree node and view the results 


**Results:**

Fit Statistics
 
Target=gender Target Label=' '
 
   Fit
Statistics    Statistics Label                Train    Validation       Test
 
  _NOBS_      Sum of Frequencies            399.000      400.000     201.000
  _MISC_      Misclassification Rate          0.439        0.480       0.547
  _MAX_       Maximum Absolute Error          0.627        0.627       0.627
  _SSE_       Sum of Squared Errors         194.907      200.632     105.345
  _ASE_       Average Squared Error           0.244        0.251       0.262
  _RASE_      Root Average Squared Error      0.494        0.501       0.512
  _DIV_       Divisor for ASE               798.000      800.000     402.000
  _DFT_       Total Degrees of Freedom      399.000         .           .
 
 
 
 
Classification Table
 
Data Role=TRAIN Target Variable=gender Target Label=' '
 
                       Target        Outcome     Frequency       Total
Target    Outcome    Percentage    Percentage      Count      Percentage
 
FEMALE    FEMALE       62.6984       38.1643         79         19.7995
MALE      FEMALE       37.3016       24.4792         47         11.7794
FEMALE    MALE         46.8864       61.8357        128         32.0802
MALE      MALE         53.1136       75.5208        145         36.3409
 
 
Data Role=VALIDATE Target Variable=gender Target Label=' '
 
                       Target        Outcome     Frequency       Total
Target    Outcome    Percentage    Percentage      Count      Percentage
 
FEMALE    FEMALE       56.0976       33.3333         69          17.25
MALE      FEMALE       43.9024       27.9793         54          13.50
FEMALE    MALE         49.8195       66.6667        138          34.50
MALE      MALE         50.1805       72.0207        139          34.75
 
 
 
 
Event Classification Table
 
Data Role=TRAIN Target=gender Target Label=' '
 
  False       True        False       True
Negative    Negative    Positive    Positive
 
   47          79          128         145
 
 
Data Role=VALIDATE Target=gender Target Label=' '
 
  False       True        False       True
Negative    Negative    Positive    Positive
 
   54          69          138         139
