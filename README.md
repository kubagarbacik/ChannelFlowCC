# ChannelFlowCC
Using AWS EC2 to compute a turbulent flow in channel with periodic hills.

The case was ispired by the following LES simulation:
http://cfd.mace.manchester.ac.uk/cgi-bin/cfddb/prcase.cgi?81&LES&database/cases/case81/Case_data&database/cases/case81&cas81_head.html&cas81_desc.html&cas81_meth.html&cas81_data.html&cas81_refs.html&cas81_rsol.html

Geometry was created in NX CAD software and exported to ANSYS Workbench to create mesh. 

Mesh file was exported to .msh ASCII format, which is operable in OpenFOAM.

Simulation was performed in steady-state, using multicore simpleFoam solver.

EC2 instance was creted with 16 cores.

To import mesh to OpenFOAM use fluentMeshToFoam command
