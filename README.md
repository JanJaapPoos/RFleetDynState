# RFleetDynState
This is a version of a Fleet Dyanmics model based on a Dynamic State Variable Model. 

It models the choice whether or not to go fishing, location choice, and discarding decisions of a fleet of fishing vessels. Fishing locations are defined by a density distribution of six size-classes of five fish species. These choices can be modelled sequentially, with up to 12 sequential time steps.  If needed, two of the species can be under individual Quota constraints at the end of the final timestep, mimicking for instance individual quotas.

Note that the package cureently only works under linux, but that before running the model, the stack size generally needs to be increased. (by using e.g. ulimit -s 256000 before starting the R session used for simulation).

In the script directory there is a simple example of using the model, demontsrating how the parameters are defined.
