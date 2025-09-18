# Fisheries distributions for SeaWise

Fisheries distributions reflect the spatial footprint of human activity in marine ecosystems and are a key consideration in the ecosystem approach to fisheries management. Where, when, and how fisheries operate not only determines the status of exploited stocks, but also affects habitats, bycatch species, and the functioning of marine ecosystems. For European seas, understanding fisheries distributions is critical for implementing the Common Fisheries Policy (CFP), meeting obligations under the Marine Strategy Framework Directive (MSFD), and supporting broader initiatives for ecosystem-based management and marine spatial planning. By analysing patterns of fishing effort in space and time, the SEAWISE project provides the evidence base needed to align fisheries management with biodiversity conservation, climate adaptation, and the sustainable use of marine resources, thereby advancing the transition towards truly ecosystem-based governance of Europe’s seas.

# A Dynamic model for fisheries distributions 
One method for learning about fisheries distributions is to model these distributions. One particular model is the Fleet Dynamics model based on a Dynamic State Variable Model. 

It models the choice whether or not to go fishing, location choice, and discarding decisions of a fleet of fishing vessels. Fishing locations are defined by a density distribution of six size-classes of five fish species. These choices can be modelled sequentially, with up to 12 sequential time steps.  If needed, two of the species can be under individual Quota constraints at the end of the final timestep, mimicking for instance individual quotas.

Note that the package cureently only works under linux, but that before running the model, the stack size generally needs to be increased. (by using e.g. ulimit -s 256000 before starting the R session used for simulation).

In the script directory there is a simple example of using the model, demontsrating how the parameters are defined.
