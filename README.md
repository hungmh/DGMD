# Run Density guided simulations for proteins using Gromacs

Usage: `./runDGMD -p PDB_File [parameters]`

Parameters:
```
	-n Number of core 
	-r Number of replica 
	-b Boxtype (cubic, dodecahedron or octahedron boxes,.. )
	-d Box Edge distance
	-t Simulation time in nanosec 
	-f Force field, type 'user' if ones wants to choose FF interactively
 	-m Reference density map file
```
Note that this automatic script  is mainly used for proteins in water. 
The protein should be approximately aligned to the reference density map before running the simulations. 
Please adjust the mdp files depending on your specific systems, particularly the *Density guided simulation* parameters in the `mdp/md.mdp`

More information: 
- https://manual.gromacs.org/current/reference-manual/special/density-guided-simulation.html
- https://manual.gromacs.org/current/user-guide/mdp-options.html#density-guided-simulations
