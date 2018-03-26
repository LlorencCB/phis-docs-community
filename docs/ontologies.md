# Ontologies

PHIS relies on two application ontologies compliant with the standards of Ontology Web Language [(OWL)](https://www.w3.org/OWL/). The ontologies are available at the Agroportal (xxxxxxxxx).

## OEPO

The Ontology for Experimental Phenotypic Objects (OEPO), allows assigning types (e.g. Experimental organization and context, Environment type, Germplasm, Physical Object) to objects involved in phenotyping experiments and defining specialization hierarchy between them according to the specificities of the installations and experiments.

The OPEPO ontology contains three main groups ob objects, namely *Experimental Context*, *Scientific Objects* and *Genetic Properties*. 

The *Experimental context* refers to the set of environmental conditions, infrastructure and supporting equipment or resources necessary to conduct a given experiment.

![oepo_expcont](img/oepo_expcont.png)

For instance, a *device* is a sub-category of *equiment* containing *vectors*, *actuators* and *sensing devices*

- *Vectors* are *devices* that either transport plants to a given site for phenotyping, or carry sensors in a greenhouse (e.g. conveyor belt, gripping arm, robot) or in the field (e.g. UAV, gantry, field robot).
By extension, a vector can also be a group of persons producing hand observations.

![oepo_vector](img/oepo_vector.png)

- *Actuators* are *devices* 

![oepo_actuator](img/oepo_actuator.png)

- *Sensing devices* are *devices* providing numerical data, e.g. environment sensors or cameras

![oepo_sensor](img/oepo_sensor.png)

- *Scientific objects* correspond to the different plant organization levels studied such as whole plants (the organism originating from a single seed, callus, rhizome or any other propagation mean), or plots (a community of plants located on a defined area of a field),but also other concepts defined at lower spatial sclae (e.g. leaf, silk, ear Inflorescence).

![oepo_scobject](img/oepo_scientificobject.png)

- Genetic material

![oepo_germplasm](img/oepo_germplasm.png)



## OEEv

The Ontology of Experimental Events (OEEv), characterises events that occur during an experiment, e.g. moving of plants, dates of sowing, application of a given treatment, harvesting, measurements or sampling for -omic measurements, or any category of technical problem.

