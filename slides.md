---
title: Uniform description and access to Knowledge Organization Systems with BARTOC and JSKOS
shorttitle: KOS description with BARTOC & JSKOS 
author: Andreas Ledl, Jakob Voß, Uma Balakrishnan
date: 2016-06-09
place: TOTh 2016 Conference, Chambéry
...


# JSKOS Knowledge Organization Systems format

## JSKOS format

* created as part of [project coli-conc](https://coli-conc.gbv.de/)\
  \ldots to provide uniform access to KOS
* based on RDF (SKOS and other ontologies)\
  \ldots but more restrictive (unification)
* based on JSON-LD\
  \ldots extended by language ranges and closed world statements
* main goal:\
  \ldots _easy use of any KOS in web applications_

## JSKOS example: GeoNames record

~~~json
{
  "uri": "http://sws.geonames.org/614540/",
  "prefLabel": {
    "en": "Georgia", 
    "fr": "Géorgie", 
    "de": "Georien", ...
  },
  "broader": [ 
    { "uri": "http://sws.geonames.org/6255147/" } 
  ],
  "inScheme": [ 
    { "uri": "http://bartoc.org/en/node/15" }
  ], ...
}
~~~

## BARTOC in JSKOS

...*fehlt noch*...

BARTOC JSKOS export: <https://github.com/gbv/bartoc-dumps/>

## JSKOS example: Eurovoc record

~~~json
{
  "uri": "http://bartoc.org/en/node/15",
  "url": "http://eurovoc.europa.eu/",
  "identifier": [ 
     "http://www.wikidata.org/entity/Q1370467" 
  ],
  "prefLabel": {
    "en": "Multilingual Thesaurus of the European Union"
  },
  "altLabel": { "en": "EuroVoc" },
  "languages": [ "bg", "ca", "cs", "da", "de", "el",
                 "en", "es", "et", "fi", "fr", ... ],
  ...
}
~~~

## JSKOS-API

* specification of HTTP API to query KOS (in JSKOS)
* based on vocabulary services use cases
* work in progress ([RDA Vocabulary Services Interest Group](https://rd-alliance.org/groups/interest-groups)?)

## JSKOS-API current state

* [Entity Lookup Microservice API (ELMA)](http://gbv.github.io/elma/)\
  \ldots most relevant subset of JSKOS-API
* public demo of terminology wrappers: 
  <https://jskos-php-examples.herokuapp.com/>
  (BARTOC, Wikidata, GND, ORCID, GeoNames, VIAF...)

## JSKOS-API example

...*fehlt noch*...

# Applications

## Applications

* uniform access to terminologies
    * browsing in knowledge organization systems
    * semantic tagging 
    * entity linking
    * ...
* terminology services
* statistical analysis of terminologies
* management of mappings
* ...

*foster the visibility, availability and usefulness of KOS in general*

## Terminology Service 

![](screenshot-normdatenservice-ddc.png)

## Mapping Database

![](mapping-db-screenshot.png)

---

## Thank you for attention

* Questions?

* Follow us on Twitter
    * [\@BARTOC_UBBasel](http://twitter.com/BARTOC_UBBasel)
    * [\@coli_conc](http://twitter.com/coli_conc)

* More information

    * <http://bartoc.org/>
    * <https://coli-conc.gbv.de/>
    * <https://gbv.github.io/jskos/>
    * <http://gbv.github.io/elma/>

*Feedback and contribution is appreciated!*

