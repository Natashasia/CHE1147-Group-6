CHE1147 — EDA SECTION 2 SUMMARY
===============================
Original records: 11,761
Distinct original SMILES strings: 8,041
Invalid/missing canonical SMILES records: 0
Duplicate canonical-SMILES rows removed (keep first): 3,720
Unique canonical structures retained: 8,041
RDKit descriptors evaluated: 217
Descriptors with any missing/nonfinite entries: 12
Missing/nonfinite entries total: 4,662 (0.267%)
Constant descriptors: 4 (SMR_VSA8, SlogP_VSA9, fr_diazo, fr_prisulfonamd)
All-missing descriptors: 0 (none)
Pairs of nonconstant descriptors with |Pearson r|>0.90: 143

Assay summary (deduplicated):
          Total  Labeled  Missing  Missing (%)  Inactive  Active  Active of labeled (%)
Assay                                                                                  
SR-ARE     8041     5611     2430         30.2      4764     847                   15.1
SR-ATAD5   8041     5551     2490         31.0      5364     187                    3.4
SR-HSE     8041     6408     1633         20.3      6082     326                    5.1
SR-MMP     8041     4419     3622         45.0      3737     682                   15.4
SR-p53     8041     5227     2814         35.0      4946     281                    5.4

IQR outlier statistics for three continuous descriptors:
            Valid_n       Q1       Q3      IQR  Lower_1p5_IQR  Upper_1p5_IQR  Potential_outliers_n  Potential_outliers_pct
Descriptor                                                                                                                
MolWt          8041  169.180  355.387  186.207       -110.131        634.698                   303                   3.768
MolLogP        8041    0.919    3.568    2.649         -3.054          7.540                   384                   4.776
TPSA           8041   26.300   80.260   53.960        -54.640        161.200                   423                   5.261

Descriptive stats for four displayed descriptors:
               mean      50%      std     min       max  skewness
MolWt       285.315  247.276  172.293  30.026  1950.681     2.519
MolLogP       2.105    2.265    2.677 -31.312    22.612    -1.244
TPSA         62.241   47.580   63.772   0.000  1095.850     4.431
NumHDonors    1.281    1.000    2.068   0.000    36.000     5.455

Strongest descriptor–descriptor pairs:
          Descriptor_1   Descriptor_2  Pearson_r  abs_r
         NumAmideBonds       fr_amide     1.0000 1.0000
              fr_Ar_NH   fr_Nhpyrrole     1.0000 1.0000
                 MolWt     ExactMolWt     1.0000 1.0000
     MaxAbsEStateIndex MaxEStateIndex     0.9999 0.9999
                Kappa2            Phi     0.9999 0.9999
                 MolWt HeavyAtomMolWt     0.9986 0.9986
        HeavyAtomMolWt     ExactMolWt     0.9986 0.9986
NumAromaticCarbocycles     fr_benzene     0.9978 0.9978

Top 20 descriptor vs. endpoint signed correlations:
                        SR-ARE  SR-ATAD5  SR-HSE  SR-MMP  SR-p53
fr_benzene               0.175     0.114   0.072   0.349   0.168
NumAromaticCarbocycles   0.175     0.115   0.071   0.348   0.169
NumAromaticRings         0.204     0.129   0.076   0.320   0.191
SMR_VSA7                 0.195     0.111   0.084   0.320   0.149
SlogP_VSA6               0.191     0.112   0.087   0.290   0.125
VSA_EState6              0.142     0.103   0.064   0.283   0.111
MolLogP                  0.141     0.039   0.112   0.273   0.067
BCUT2D_LOGPHI            0.158     0.050   0.076   0.272   0.154
fr_Ar_OH                 0.130     0.081   0.065   0.259   0.123
fr_phenol                0.133     0.083   0.068   0.259   0.128
fr_phenol_noOrthoHbond   0.136     0.083   0.071   0.259   0.126
SMR_VSA9                 0.153     0.111   0.035   0.233   0.143
RingCount                0.178     0.096   0.046   0.228   0.195
BertzCT                  0.198     0.087   0.054   0.227   0.195
FpDensityMorgan1        -0.142    -0.076  -0.083  -0.222  -0.099
SlogP_VSA11              0.114     0.076   0.031   0.218   0.120
AvgIpc                   0.179     0.066   0.050   0.209   0.146
FractionCSP3            -0.149    -0.118  -0.070  -0.207  -0.106
MolMR                    0.164     0.054   0.072   0.206   0.160
PEOE_VSA7                0.095     0.030   0.059   0.205   0.124

NOTE: Duplicate structures keep FIRST row without merging labels.
NOTE: Correlations were examined for EDA visualization only.
NOTE: No final ML feature selection or train/test preprocessing is performed here.