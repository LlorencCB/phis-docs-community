# Ontologies

PHIS relies on two application ontologies compliant with the standards of the [**Ontology Web Language**](https://www.w3.org/OWL/ "OWL"). The ontologies are available at the [**Agroportal**](http://agroportal.lirmm.fr/ "Agroportal").

## OEPO

The **Ontology for Experimental Phenotypic Objects (OEPO)**, allows assigning types (e.g. Experimental organization and context, Environment type, Germplasm, Physical Object) to objects involved in phenotyping experiments and defining specialization hierarchy between them according to the specificities of the installations and experiments.

The OEPO ontology contains three main groups of objects, namely *Experimental Context*, *Scientific Objects* and *Genetic Properties*.

### Experimental context

The *Experimental context* refers to the set of environmental conditions, infrastructure and supporting equipment or resources necessary to conduct a given experiment in which plants, plots or group of plants are raised.

A number of the terms and definitions follow recommendations adopted by the ESFRI listed project [**EMPHASIS**](emphasis_ontology.md "EMPHASIS ontology") and reuses accepted terms for establishing relations and describing experiments from OBO foundry such as the [**Plant Experimental Conditions Ontology**](http://purl.bioontology.org/ontology/PECO).

![oepo_expcont](img/oepo_expcont.png "Experimental context")

For instance, a *device* is a sub-category of *equiment* containing *vectors*, *actuators* and *sensing devices*

- *Vectors* are *devices* that either transport plants to a given site for phenotyping, or carry sensors in a greenhouse (e.g. conveyor belt, gripping arm, robot) or in the field (e.g. UAV, gantry, field robot).
By extension, a vector can also be a group of persons producing hand observations.

![oepo_vector](img/oepo_vector.png)

- *Actuators* are *devices* that usually are responsible for moving and controlling a mechanism or system, for example by opening a valve or opening shadows in a greenhouse.

![oepo_actuator](img/oepo_actuator.png)

- *Sensing devices* are *devices* providing numerical data, e.g. environment sensors or cameras. Environmental sensors follow the [**Semantic Sensor Network Ontology**](http://purl.oclc.org/NET/ssnx/ssn "SSN ontology"). For instance, a *Quantum sensor* is a *sensing device* and a sub-type of *Radiation sensor*.

![oepo_sensor](img/oepo_sensor.png)

### Scientific objects

 *Scientific objects* correspond to the different plant organization levels studied such as *whole plants* (the organism originating from a single seed, callus, rhizome or any other propagation mean), or *plots* (a community of plants located on a defined area of a field), but also other concepts defined at lower spatial scale (e.g. *leaf*, *silk*, *ear Inflorescence*). Terms present in this ontology map onto existing ontologies providing relevant concept hierarchies related to the anatomy, structure and phenotype of plants described in the [**Planteome project**](http://planteome.org/ "Planteome")<sup>1</sup> such as the [**Crop Ontology**](http://cropontology.org/ "Crop ontology")<sup>2</sup>, the [**Plant Ontology**](http://plantontology.org/ "Plant Ontology")<sup>3,4,5</sup>, the [**PATO**](http://www.obofoundry.org/ontology/pato.html "PATO"), the [**PPEO**](http://wheat.agroportal.lirmm.fr/ontologies/PPEO "PPEO"), and other ontological resources such as the [**AGROVOC**](http://artemide.art.uniroma2.it:8081/agrovoc/agrovoc/en/ "AGROVOC")<sup>6</sup>. 

![oepo_scobject](img/oepo_scientificobject.png)

### Genetic properties

 *Genetic properties* refer to the different attributes related to a germplasm entity incuding the *Genus*, *Species*, *AccessionName*, *AccessionNumber*, *Variety*, *Seedlot* and *SeedLotSample*. These attributes follow the [**FAO/Bioversity Multi Crop Passport Descriptors**](https://www.bioversityinternational.org/e-library/publications/detail/faobioversity-multi-crop-passport-descriptors-v21-mcpd-v21/ "FAO/Bioversity Multi Crop Passport Descriptors")<sup>7,8</sup>.

![oepo_germplasm](img/oepo_germplasm.png)

## OEEv

The **Ontology of Experimental Events (OEEv)**, characterises  events that occur during an experiment, e.g.  dates of sowing, application of a given treatment, harvesting, measurements or sampling for -omic measurements, or any category of technical problem. The OEEv ontology contains **five** groups of events, namely *Facicility Management*, *Scientific Object Management*, *Phenology*, *Trouble* and *Displacement*.

### Facility Management

The *Facility Management* refers to the set of actions related to the management and maintenance infrastructure and supporting equipment. It describes events related to *servicing*, *maintenance* and *calibration* of *equipment* or *installations*.

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

### Phenology

The *Phenology* refers to the set of events related to the different phenological stages of plants.

### Trouble

The event *Trouble* is defined by three different sub-categories:

- *Breakdown* (sensor or conveyor)
- *Dysfunction* (sensor fault, irrigation trouble)
- *Incident* (a pot falls down, a leaf is blocked in an imaging cabin, lodging of a plot, human error, etc.)

![trouble](img/oeev_trouble.png "Trouble")

Several subtypes of incidents that ofter occur in platfortm or field experiments have been declared including:

- *PotFall*
- *Lodging*
- *StuckPlant*
- *PestAttack* 

![incidents](img/incidents.png "Incidents")

### Displacement (object tracking)

The *Displacement* event has been created to follow the position in time and space of the different objects participating in experiments. For instance, plants are often transferred, during a single experiment, between installations or compartments with different environmental conditions. Similarly, sensors can be replaced or moved to different positions in the field or greenhouse.
The *MoveTo* and *MoveFrom* concepts allow tracking objects:

![displacement](img/oeev_displacement.png "object displacement")

Events or simple annotations are annotated as shown in the following diagram following the [**Web Annotation Data Model**](https://www.w3.org/TR/annotation-model/) that allows assigning motivation and purpose attributes to annotations (e.g. oa:describing, oa:identifying, oa:linking, oa: replying, etc.). [**Dublin Core**](http://dublincore.org/) properties such as **dcterms:created** or **dcterms:creator** are also used.

![annotexample](img/example_annotation.png)

- Instances are depicted as coloured ellipses.
- Classes are depicted as white rectangles.
- Literals are depicted as white lozenges.
- Relationships and properties are depicted as black lines.
    
## Use case

The following semantic graph represents how [**OEPO**](ontologies#oepo) and [**OEEv**](ontologies#oeev) ontologies interact for representing some of the characteristics and events of plot 97 in the field experiment DIA2017-05-19.

Thus, the ***plot97*** is of type ***plot***, participates in the experiment ***DIA2017-05-19***, and has a spatial geometry (***GPScoord***) defined following the [**Well-known text standard**](https://en.wikipedia.org/wiki/Well-known_text). ***plot97*** contains the ***plant144*** (which is of type ***plant***) which in turn contains ***leaf461*** (which is of type ***leaf***). All these temrms and semantic relationships between objects are defined following the [**OEPO**](ontologies#oepo) ontology. On the other hand, [**OEEv**](ontologies#oeev) ontology allows describing events cocerning the different obejects involved in an experiment. In the example presented here, the ***event54*** that concerns ***plot97*** is of type ***Incident*** and occurred the **"2017-06-29"**. ***event54*** is associated to the ***anno65*** which is of type ***Annotation***. This annotation, has a creator (***Romain***), a date of annotation (**"2017-08-10"**) and a body value describing the event (**"Plot lodged after the storm"**).

![example_oepo_oeev](img/example_oepo_oeev.png)

- Instances are depicted as coloured ellipses.
- Classes are depicted as white rectangles.
- Literals are depicted as white lozenges.
- Relationships and properties are depicted as black lines.

For better legibility objects are labelled with shortened alias names rather than using full URIs:

- ***plot97***: http://www.phenome-fppn.fr/diaphen/2017/o17000097
- ***plant471***: http://www.phenome-fppn.fr/diaphen/2017/17000471
- ***leaf1820***: http://www.phenome-fppn.fr/diaphen/2017/l17001820
- ***DIA2017-05-19***: http://www.phenome-fppn.fr/diaphen/DIA2017-05-19
- ***GPScoord***: Polygon ((3.973276 43.61203, 3.973306 43.61201, 3.973354 43.61205, 3.973324 43.61207, 3.973276 43.61203))
- ***Romain***: chapuis@supagro.inra.fr
- ***event54***: http://www.phenome-fppn.fr/diaphen/eventInsertion_DIA2017-05-19event_3788430f-300a-4c30-8dff-2bdf7bcd9e49
- ***anno65***: http://www.phenome-fppn.fr/diaphen/eventInsertion_DIA2017-05-19anno_22d75679-38de-4c58-b505-23ed39e180fa

Note that not all objects and events associated to ***plot97*** are represented in this graph. Fulls details can be found in the PHIS user interface by searching for plot 97 in the different menus (e.g. **Events**, **Scientific objects**).

## References

<sup>1</sup>Cooper L, Meier A, Laporte MA, Elser JL, Mungall C, Sinn BT, Cavaliere D, Carbon S, Dunn NA, Smith B, et al. 2018. The Planteome database: an integrated resource for reference ontologies, plant genomics and phenomics. *Nucleic Acids Research* 46: D1168-D1180.

<sup>2</sup>Shrestha R. 2012. Bridging the phenotypic and genetic data useful for integrated breeding through a data annotation using the CropOntology developed by the crop communities of practice. *Frontiers in Physiology* 3.

<sup>3</sup>Cooper L, Walls RL, Elser J, Gandolfo MA, Stevenson DW, Smith B, Preece J, Athreya B, Mungall CJ, Rensing S. 2013. The plant ontology as a tool for comparative plant anatomy and genomic analyses. *Plant and Cell Physiology* 54: e1-e1.

<sup>4</sup>Ilic K, Kellogg EA, Jaiswal P, Zapata F, Stevens PF, Vincent LP, Avraham S, Reiser L, Pujar A, Sachs MM, et al. 2007. The plant structure ontology, a unified vocabulary of anatomy and morphology of a flowering plant. *Plant Physiology* 143: 587-599.

<sup>5</sup>Walls RL, Athreya B, Cooper L, Elser J, Gandolfo MA, Jaiswal P, Mungall CJ, Preece J, Rensing S, Smith B. 2012. Ontologies as 
integrative tools for plant science. *American Journal of Botany* 99: 1263-1275.

<sup>6</sup>Caracciolo C, Stellato A, Morshed A, Johannsen G, Rajbhandari S, Jaques Y, Keizer J. 2013. The AGROVOC linked dataset. *Semantic Web* 4: 341-348.

<sup>7</sup>Alercia A, Diulgheroff S, Mackay M 2015. FAO/Bioversity Multi-Crop Passport Descriptors V. 2.1 [MCPD V. 2.1]-December 2015: Bioversity International.

<sup>8</sup>Yeumo ED, Alaux M, Arnaud E, Aubin S, Baumann U, Buche P, Cooper L, Ćwiek-Kupczyńska H, Davey RP, Fulss RA. 2017. Developing data interoperability using standards: A wheat community use case. *F1000Research* 6.
