# Ontologies

PHIS relies on two application ontologies compliant with the standards of the [**Ontology Web Language**](https://www.w3.org/OWL/ "OWL"). The ontologies are available at the [**Agroportal**](http://agroportal.lirmm.fr/ "Agroportal").

## OEPO

The **Ontology for Experimental Phenotypic Objects (OEPO)**, allows assigning types (e.g. Experimental organization and context, Environment type, Germplasm, Physical Object) to objects involved in phenotyping experiments and defining specialization hierarchy between them according to the specificities of the installations and experiments.

The OEPO ontology contains three main groups of objects, namely *Experimental Context*, *Scientific Objects* and *Genetic Properties*.

### Experimental context

The *Experimental context* refers to the set of environmental conditions, infrastructure and supporting equipment or resources necessary to conduct a given experiment. 

A number of the terms and definitions follow recommendations adopted by the ESFRI listed project [**EMPHASIS**](emphasis_ontology.md "EMPHASIS ontology").

![oepo_expcont](img/oepo_expcont.png "Experimental context")

For instance, a *device* is a sub-category of *equiment* containing *vectors*, *actuators* and *sensing devices*

- *Vectors* are *devices* that either transport plants to a given site for phenotyping, or carry sensors in a greenhouse (e.g. conveyor belt, gripping arm, robot) or in the field (e.g. UAV, gantry, field robot).
By extension, a vector can also be a group of persons producing hand observations.

![oepo_vector](img/oepo_vector.png)

- *Actuators* are *devices* that usually are responsible for moving and controlling a mechanism or system, for example by opening a valve or opening shadows in a greenhouse.

![oepo_actuator](img/oepo_actuator.png)

- *Sensing devices* are *devices* providing numerical data, e.g. environment sensors or cameras. Environmental sensors follow the [**Semantic Sensor Network Ontology**](http://purl.oclc.org/NET/ssnx/ssn "SSN ontology").

![oepo_sensor](img/oepo_sensor.png)

### Scientific objects

 *Scientific objects* correspond to the different plant organization levels studied such as *whole plants* (the organism originating from a single seed, callus, rhizome or any other propagation mean), or *plots* (a community of plants located on a defined area of a field), but also other concepts defined at lower spatial scale (e.g. *leaf*, *silk*, *ear Inflorescence*). Terms present in this ontology map onto existing ontologies providing relevant concept hierarchies related to the anatomy, structure and phenotype of plants described in the [**Planteome project**](http://planteome.org/ "Planteome")<sup>1</sup> such as the [**Crop Ontology**](http://cropontology.org/ "Crop ontology")<sup>2</sup>, the [**Plant Ontology**](http://plantontology.org/ "Plant Ontology")<sup>3,4,5</sup>, the [**PATO**](http://www.obofoundry.org/ontology/pato.html "PATO"), and other ontological resources such as the [**AGROVOC**](http://artemide.art.uniroma2.it:8081/agrovoc/agrovoc/en/ "AGROVOC")<sup>6</sup>. 

![oepo_scobject](img/oepo_scientificobject.png)

### Genetic properties

 *Genetic properties* refer to the diffrent attributes related to a germplasm entity such as the *species*, *genotype* or the *seedlot*. The [**FAO/Bioversity Multi Crop Passport Descriptors**](https://www.bioversityinternational.org/e-library/publications/detail/faobioversity-multi-crop-passport-descriptors-v21-mcpd-v21/ "FAO/Bioversity Multi Crop Passport Descriptors")<sup>7,8</sup> is also used for germplasm identification.

![oepo_germplasm](img/oepo_germplasm.png)

## OEEv

The **Ontology of Experimental Events (OEEv)**, characterises events that occur during an experiment, e.g.  dates of sowing, application of a given treatment, harvesting, measurements or sampling for -omic measurements, or any category of technical problem. The OEEv ontology contains four groups of events, namely *Facicility Management*, *Scientific Object Management*, *Trouble* and *Displacement*.

### Facility Management

The *Facility Management* refers to the set of actions related to the manage and maintenance infrastructure and supporting equipment. It describes events related to *servicing*, *maintenance* and *calibration* of *equipment* or *installations*.

![facility_management](img/oeev_facilitymanagement.png "facility_management")

![facility_management2](img/oeev_operability.png "facility_management")

### Scientific Object Management

The *Scientific Object Mangament* contains different sub-categories of events related to the typical operations conducted on plants or plots in experiments:

- *AddingProduct* refers to the application of products such as fertilizers
- *Clipping* is related to the installation of accessories surch as embeded sensors
- *Thinning* refers to the removal of some plants, or parts of plants, to make room for the growth of others
- *Treatment* related to either *curative* or *preventive* treatments applied to plants
- *Potting* aplies to pot experiments
- *Sowing* applies for both field and pot experiments
- *Stacking* refers to the action of putting plant tutors

![scientificobject](img/oeev_scientific_object_management.png "Scientific Object Management")

### Trouble

The event *Trouble* is defined by three different sub-categories:

- *Breakdown* (sensor or conveyor)
- *Dysfunction* (sensor fault, irrigation trouble)
- *Incident* (a pot falls down, a leaf is blocked in an imaging cabin, lodging of a plot, human error, etc.)

![trouble](img/oeev_trouble.png "Trouble")

### Displacement (object tracking)

The *Displacement* event has been created to follow the position in time and space of the different objects participating in experiments. For instance, plants are often transferred, during a single experiment, between installations or compartments with different environmental conditions. Similarly, sensors can be replaced or moved to different positions in the field or greenhouse.
The *MoveTo* and *MoveFrom* concepts allow tracking objects:

![displacement](img/oeev_displacement.png "object displacement")

### References

<sup>1</sup>Cooper L, Meier A, Laporte MA, Elser JL, Mungall C, Sinn BT, Cavaliere D, Carbon S, Dunn NA, Smith B, et al. 2018. The Planteome database: an integrated resource for reference ontologies, plant genomics and phenomics. *Nucleic Acids Research* 46: D1168-D1180.

<sup>2</sup>Shrestha R. 2012. Bridging the phenotypic and genetic data useful for integrated breeding through a data annotation using the CropOntology developed by the crop communities of practice. *Frontiers in Physiology* 3.

<sup>3</sup>Cooper L, Walls RL, Elser J, Gandolfo MA, Stevenson DW, Smith B, Preece J, Athreya B, Mungall CJ, Rensing S. 2013. The plant ontology as a tool for comparative plant anatomy and genomic analyses. *Plant and Cell Physiology* 54: e1-e1.

<sup>4</sup>Ilic K, Kellogg EA, Jaiswal P, Zapata F, Stevens PF, Vincent LP, Avraham S, Reiser L, Pujar A, Sachs MM, et al. 2007. The plant structure ontology, a unified vocabulary of anatomy and morphology of a flowering plant. *Plant Physiology* 143: 587-599.

<sup>5</sup>Walls RL, Athreya B, Cooper L, Elser J, Gandolfo MA, Jaiswal P, Mungall CJ, Preece J, Rensing S, Smith B. 2012. Ontologies as 
integrative tools for plant science. *American Journal of Botany* 99: 1263-1275.

<sup>6</sup>Caracciolo C, Stellato A, Morshed A, Johannsen G, Rajbhandari S, Jaques Y, Keizer J. 2013. The AGROVOC linked dataset. *Semantic Web* 4: 341-348.

<sup>7</sup>Alercia A, Diulgheroff S, Mackay M 2015. FAO/Bioversity Multi-Crop Passport Descriptors V. 2.1 [MCPD V. 2.1]-December 2015: Bioversity International.

<sup>8</sup>Yeumo ED, Alaux M, Arnaud E, Aubin S, Baumann U, Buche P, Cooper L, Ćwiek-Kupczyńska H, Davey RP, Fulss RA. 2017. Developing data interoperability using standards: A wheat community use case. *F1000Research* 6.
