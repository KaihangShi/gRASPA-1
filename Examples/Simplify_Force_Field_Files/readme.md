Cleaning up (simplify) the force field files using python scripts. 
It reads what framework/adsorbates you are going to use, and remove every unused element from the files below. 

-- force_field_mixing_rules.def
-- pseudo_atoms.def

This can reduce the time to process the force field parameters and MAY give you a little speed up. It reduces memory required as well. 

** NOTE **
1. The example starts with the force_field_mixing_rules.def file using the UFF/TraPPE.
2. For overwritting terms (force_field.def, like tail corrections), you need to manually add them, the python script does not do it for you. 
3. For the partial charges in the pseudo_atoms.def file, they are zero. After running the python script, please input the charges according to your model. 
