This readme file describes the folder structure for the sub-folder: /DATA/GROMACS/
!-------------------------------------!

/WATER/

The sub-folders here contains simulations of either bulk water or vapor deposition simulations of water on a substrate.
!-------------------------------------!

/WATER/Bulk/

The bulk water folder has sub-folders for simulations for either Gas-liquid critical point or liquid-liquid critical point 
!-------------------------------------!


/WATER/Gas_liquid_cp/

The sub-folders describes the ensemble information used, e.g., NVT (canonical ensemble) or NPT (isothermal-isobaric ensemble).

Then the sub-folder are based on the number of molecules used, temperature and/or pressure etc. All the folders containing the simulation data contains an analysis folder containing the plots and output data of the analysis codes. The analysis codes are called from /DATA/analysis_codes/..
!-------------------------------------!

/WATER/Vapor_deposition/

The vapor_deposition contains sub-folders describing the box size (the ensemble used is always NVT). The sub-folders then describe the interaction strength parameter used for wall oxygen interactions and then the particle insertion protocol used, either /random_vel or /speed_of_sound, which corresponds to either random velocity assignment to particles or a velocity of sound towards the substrate.
!-------------------------------------!

An example:

/WATER/
    /Bulk
	/Liquid_liquid_cp
	/Gas_liquid_cp
	    /NPT
		/...
	    /NVT
		/...
    /Vapor_deposition
	/Box_20_20_100
	    /f1
		/random_vel
		/speed_of_sound
	    /f8
	/Box_40_40_200