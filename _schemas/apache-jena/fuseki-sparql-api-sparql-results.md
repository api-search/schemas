---
description: SPARQL query results in JSON format
layout: schema
name: SparqlResults
properties_list:
- description: Result metadata including variable names
  name: head
  type: object
- description: Query result bindings
  name: results
  type: object
- description: Result for ASK queries
  name: boolean
  type: boolean
provider_name: Apache Jena
provider_slug: apache-jena
schema_file: json-schema/fuseki-sparql-api-sparql-results-schema.json
slug: fuseki-sparql-api-sparql-results
tags:
- Java
- Linked Data
- OWL
- Ontology
- Open Source
- RDF
- Semantic Web
- SPARQL
title: SparqlResults
---
