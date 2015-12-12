# MappingSchemaDotOrg2DBpedia
Manual created mapping between the ontologies
[Schema.org](http://schema.org) and [DBpedia](http://dbpedia.org). This mapping involves the URIs http://drop and http://resolve. The drop-URI is meant for instances which can be present in Schema.org (e.g. Offers) but not in DBpedia as DBpedia provides users with information from Wikipedia which is limited to 'related' information.

The URI http://resolve exists because of the different hierarchy-levels in the ontologies. While DBpedia is rather flat, Schema.org tends to be more nested. For example, an instance in DBpedia directly holds GPS coordinates while in Schema.org an extra instance exists. The class of the instance would be marked as http://resolve and by this, the transformer (To be released) should take the properties (e.g. GPS coordinates) and move them to the parent instance.

## Caution
This mapping was created manually without taking care of range or domain. 

## Use Case
You do not know what to do with this project? Check out my [blog post on LOMI](https://www.maximilian-boehm.com/hp2125/LOMI-Enrich-Linked-Open-Data-DBpedia-with-Microdata.htm).
