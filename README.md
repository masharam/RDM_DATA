# RDM_DATA
Research Data Management workshop (09.10.2024 retreat)

This text file describes the outer layer of folder structure for my simulation data. 

The /DATA/ folder contains 3 folders, one contains all the analysis codes, and 2 other folders based on what software (e.g., LAMMPS or GROMACS) was used to generate the data.

Inside of each of these folders, the sub-folders are for different systems (LJ, Water etc.) that are being simulated. 

Further inside, these folders have specific folder structure which is described in a $path_README.txt file inside those folders.

an example for the folder structure:

/DATA/
    /analysis_codes/
        /LAMMPS/
	/GROMACS/
	    /...
    /LAMMPS/
        /...
    /GROMACS/
        /LJ/
	    GROMACS_LJ_README.txt
	    /Cubic_Box/
	    /Elongated_Box_3_1_1/
	/WATER/
	    GROMACS_WATER_README.txt
	    /Bulk/
		/Liquid_liquid_cp/
		/Gas_liquid_cp/
		    /NPT/
		    /NVT/
			/N683/
			/N1225/
			    /T680/
			    /T690/
			        /analysis/
	    /Vapor_deposition/
		/Box_20_20_100/
		    /...
		/...
