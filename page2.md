
# Technical Documentation OIMS Beta 1.1.1

## Table of contents

[1.	Introduction](#1-introduction)

[2.	Metadata for making data FAIRER](#2-metadata-for-making-data-fairer)

[3.	Metadata schemas for describing metadata schemas](#3-metadata-schemas-for-describing-metadata-schemas)

[4.	Data entity linkages metadata](#4-data-entity-linkages-metadata)

## 1.	Introduction
Open data era and the CGIAR Platform mission to harness the capabilities of big data to accelerate and enhance the impact of international agricultural research for development. The data is there but is very often underutilized, because the data is not interoperable or reusable. 
Why OIMS.
There are two ways of inderstanding what is happening:
1.	Top down: what are we trying to achieve
2.	Bottom up: can we build up a generic metadata schema

### 1.1.	The choice of JSON
Why we choose JSON as our format.

### 1.2.	FAIRER data standards
Key definitions:
FAIRER
**F**indable<br>
**A**ccessible<br>
**I**nteroperable<br>
**R**eusable<br>
**E**thical or responsible<br>
**R**eproducible<br>

### 1.3.	Data entities
The notion of data entities is based on the fact that what we understand by data varies. At a high level of aggregation we have data collections or studies. These may have sub-collections. Within this concept we have data sets. Data sets are groupings of one or more files with a persistent identifier. The files are the tangible assets and within those files we can have things like tables, variables and records. It is clear that there is a hierarchy amongst the data entities. Not all entity types are relevant for each case we are describing. Moreover, we distinguish between primary secondary and metadata data entities. Primary data entities Are core data entities such as collections, data sets, data files, tables, variables. The secondary data entities are supporting documentation and information linked to a primary data entity. Any data entity can have metadata. In order to understand how these ata entities are related we need to document this in a standardized form.
 
## 2.	Metadata for making data FAIRER
The type of metadata provided with data entities depends critically on the data entity provider as well as on some key domain issues.<br>
Example of machine data loss.

### 2.1.	Findable

Descriptive aspect metadata<br> 
Technical aspect metadata<br>
### 2.2.	Accessible
Descriptive aspect metadata <br>
Technical aspect metadata<br>

### 2.3.	Interoperable
Descriptive aspect metadata <br>
Technical aspect metadata<br>
Structural metadata<br>
### 2.4.	Reusable
Descriptive aspect metadata <br>
Technical aspect metadata<br>
Structural metadata<br>

### 2.5.	Ethical or Responsible
Descriptive aspect metadata <br>
Technical aspect metadata<br>
Structural metadata<br>

### 2.6.	Reproducible 
Descriptive aspect metadata <br>
Technical aspect metadata<br>

 
## 3.	Metadata schemas for describing metadata schemas
In order to describe a metadata schema we need a format for doing so.<br>
Each metadata field can be described with the following elements<br>
+  AttributeName: the identifier of the metadata field<br>
+  AttributeDescription: A short description of what the metadata field entails<br>
+  DataType: the data type of the contents of the metadata field<br>
+  Format: if applicable a specific format of the metadata field<br>
+  Status: determine if a field is: required; recommended; required if applicable; recommended if applicable; optional<br>
+  TypeClass: identification if a metadata field consists of multiple attributes or is the attribute sufficiently granular<br>
+  Multiple: does a metadata field allow multiple entries or not<br>
+  OntologyTerm: attribute value identifier<br>
   -  OntologyTermName: ontology term human readable<br>
   -  OntologyTermDescription: <br>
   -  OntologyName<br>
   -  OntologyTermID<br>
   -  OntologyTermURL<br>
   -  OntologyTermQuality<br>

If the data type is enumeration, then there is a controlled vocabulary linked to that field<br>
+  ControledVocabulary: description of the controlled vocabulary<br>
   -  VocabularyElementID: element identifier<br>
   -  VocabularyElementDescription: description of the element<br>
   -  OntologyTerm: element identifier<br>
      =  OntologyTermName: ontology term human readable<br>
      =  OntologyTermDescription: <br>
      =  OntologyName<br>
      =  OntologyTermID<br>
      =  OntologyTermURL<br>
      =  OntologyTermQuality<br>


We can therefore describe the elements of the metadata-metadata in the same terms as well, albeit that these may contain different elements depending on the schema. In the end we can describe the elements of the metadata-metadata-metadata in terms of themselves which then becomes the basis for the description of any metadata schema.  
So at the highest level of abstraction we have a metadata schema that describes itself. We can use this schema to describe any metadata of metadata schemas that may contain additional elements. 
That schema can be used to describe the metadata schema that is used to describe data entitities. 
In addition to the 9 major attributes and the 8 attribute attributes there is one more that we use, namely the attribute “//” which we use as a comment 


### 3.1.	High level of abstraction metadata schema
We use the metadata attributes to describe the most essential metadata attributes mentioned at the beginning of the Chapter. This is a metadata schema that describes itself only. It can be used as a basis for any other metadata schema.
https://github.com/GideonKruseman/CGIAR_BigData_metadata_schema/blob/master/MetaDataMetaDataStructureOIMSversionBeta1_1.json
It covers the following attributes, the only special one is comment because it is not necessary for the schema to be machine readable. We are staunch believers of documenting code and this allows us to document the code.
Comment
+  AttributeName
+  AttributeDescription
+  Status
+  TypeClass
+  Multiple
+  DataType
+  ControlledVocabulary
+  VocabuaryElementName
+  VocabularyElementDescription
+  OntologyTerm
+  OntologyTermName
+  OntologyTermDescription
+  OntologyTermID
+  OntologyTermURL
+  OntologyTermQuality
+  AttributeValueElements

### 3.2.	Intermediate level of abstraction metadata schema 
Using the high level of abstraction metadata-schema it is possible to describe an intermediate level metadata schema. Usually, this will contain all the same elements of the high abstract schema plus any other attributes used to describe the actual metadata schema attributes. Remember that the high level of abstraction metadata schema only describes itself so there are certain elements that it cannot describe, for instance data types that are not used in the metadata-metadata of the metadata structure. 
Some key additional components of the intermediate level of abstraction metadata schema include: the definition of any datatypes  identified in the metadata schema.

 
## 4.	Data entity linkages metadata


