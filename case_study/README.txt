This file will briefly include each step in the workflow, and a short description of what it is.
For each step, a separate folder will be made, where all final results and scripts will lie.

Note:- Steps are not necessarily in order of their flow of data 

@Veda
step_01 -> EC_class2_data.json file will be used to fetch PDB files and predict binding sites using COACH 

@Veda
step_02 -> EC_class2_data.json file will be used to prepare .mol2 files using GYPSUM

@Veda
step_03 -> Using data from step_01 and step_02 above, docking simulations of each enzyme with their corresponding substrates will be performed using autodock. The output of this step will be 3d-coordinates of complex for each Enzyme-substrate pair and the binding affinity 

@
step_04 -> Will utiliize outputs from step_01 above to construct 3D-grids of coordinates (similar to https://github.com/pulimeng/DeepDrug3D) and use outputs from step_03 above to construct 3D-grids of energy potentials (similar to https://github.com/DS3Lab/RosENet)

@
step_05 -> Will utilize grids from step_04 above to formulate a CNN that can a). classify enzymes as promiscuous or not based on 3D-grids of coordinates above  b). classify enzymes as promiscuous or not based on 3D-grids of energy potentials above c). classify enzymes as promiscuous or not based on 3D-grids of coordinates and 3D-grids of energy potentials

@ 
step_06 -> (If necessary), construct an ensemble model utilizing CNN model above in addition to sequence model that @Deepro developed already

Outcomes :- 
1. We will understand if just using 3d-coordinates 


