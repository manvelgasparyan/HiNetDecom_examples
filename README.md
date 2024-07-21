# Nested hierarchical decomposition for two real-life biomodels b2AR and EGFR.

This GitHub repository contains a Python implementation of the nested hierarchical decomposition for the models of B2AR and EGFR. This package corresponds to the journal article "Hierarchical Optimization of Biochemical Networks", which is publicly available at "the link goes here." For more details, please refer to that paper.

The package includes six SBML files corresponding to two biomodels: b2AR_PKA_v5 and D4_model_EGFR_v13b. Each model has three associated files:

1. b2AR_PKA_v5_original.xml - This SBML file represents the original model1.
2. b2AR_PKA_v5_removed_reaction.xml - This SBML file represents the original model1 with certain reversible reactions modified     to be irreversible (refer to the cited journal article for details).
3. b2AR_PKA_v5_reduced.xml - This SBML file represents the Michaelis-Menten reduced version of model1 with specific reactions      removed as mentioned.
   
Similarly, the files for EGFR are:

1. D4_model_EGFR_v13b_original.xml
2. D4_model_EGFR_v13b_removed_reaction.xml
3. D4_model_EGFR_v13b_reduced.xml

The Python package accepts an SBML file (either 'b2AR_PKA_v5_reduced.xml' or 'D4_model_EGFR_v13b_reduced.xml') as input and produces hierarchical levels of species subsets. Each subset is nested within the next, collectively forming the complete decomposition.
