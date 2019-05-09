# Managing the data lake
[![CIMMYT](https://www.logolynx.com/images/logolynx/cf/cf14c764d6ef4df851292c2ac93b5e97.png)](https://www.cimmyt.org/)
[![CopSED](https://bigdata.cgiar.org/wp-content/uploads/2018/12/SOCIO-ECONOMIC-DATA_Big-Data-Icon-280px.png)](https://bigdata.cgiar.org/communities-of-practice/socio-economic-data/)
[![BDP](https://bigdata.cgiar.org/wp-content/uploads/2017/06/CGIAR_PforBD-Orange-logo220.png)](https://bigdata.cgiar.org/)


As a staunch believer in **Open Access**, **Open Data**, and **Open Source** it is imperative to make sure that things are actually usable. Key concept for making that possible is the [data lake](https://www.cimmyt.org/blogs/big-data-for-development-research/). [Read more...](https://www.linkedin.com/pulse/data-swamp-versus-lake-world-where-warehouses-seem-kruseman-phd/)

This webpage provides links to the technical implementation of methods to navigate the data lake, the bait you need to fish for data in the lake and the appropriate gear to do.

## At a glace
[OIMS Metadata schema](https://gideonkruseman.github.io/#OIMS-Metadata-schema) 

[ETL-procedures](https://gideonkruseman.github.io/#ETL-procedures) 

## OIMS Metadata schema
The key for manging the data lake is good metadata. However for that metadata to be useable it needs to be interoperable and machine-actionable. At the same time it needs to be human-readable, otherwise no one will be able to use it. We have been developing a metadata schema to do just that. OPIMS is a human-readable, machine-actionable flexible and extensible, ontology-independent metadata schema focused on making messy socio-economic data FAIRER. FAIRER stands for *F*indable, *A*ccessible, *I*nteroperable, *R*eusable, *E*thical and responsible, *R*eproducible guidelines for data. It builds on the [FAIR data guidelines](https://www.nature.com/articles/sdata201618), but takes it further.

The development of the OIMS metadata schema is on [Github](https://github.com/GideonKruseman/CGIAR_BigData_metadata_schema), check it out for the latest developments. The launch date is planned for late June, 2019.

The OIMS metadata schema is based on *J*ava*S*cript *O*bject *N*otation ([JSON](https://www.json.org/)).



### Central concepts of OIMS
**Data entities**
The notion of data entities is based on the fact that what we understand by data varies. At a high level of aggregation we have data collections or studies. These may have sub-collections. Within this concept we have data sets. Data sets are groupings of one or more files with a persistent identifier. The files are the tangible assets and within those files we can have things like tables, variables and records. It is clear that there is a hierarchy amongst the data entities. Not all entity types are relevant for each case we are describing. Moreover, we distinguish between primary secondary and metadata data entities. Primary data entities Are core data entities such as collections, data sets, data files, tables, variables. The secondary data entities are supporting documentation and information linked to a primary data entity. Any data entity can have metadata. In order to understand how these ata entities are related we need to document this in a standardized form.

### OIMS core: metadata schema that describes itself


### the link with ontologies



## ETL procedures
*E*xtract, *T*ransform and *L*oad procedures are at the core of making data stored in a lake reusable. Actually ETL proceduresare every where. We use them at the back-end and at the front-end

## Contact
![Gideon](https://gallery.mailchimp.com/59a7500ef5c94dd50e2b9e2fb/images/7519ddc6-0c01-4d8c-b437-9c82670cd75a.png) 

**Gideon Kruseman**

Community of practice lead

[Community of Practice on Socio-economic data](https://bigdata.cgiar.org/communities-of-practice/socio-economic-data/)

[CGIAR Platform for Big Data in Agriculture](https://bigdata.cgiar.org/)

[email](mailto:g.kruseman@cgiar.org)


**CoP SED secretariat**

[email](mailto:cgiar.cop.sed@gmail.com)





