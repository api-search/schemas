---
description: An RDF term (URI, literal, or blank node)
layout: schema
name: RDFTerm
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: value
  type: string
- description: Datatype URI for typed literals
  name: datatype
  type: string
- description: Language tag for language-tagged literals
  name: xml:lang
  type: string
provider_name: Apache Jena
provider_slug: apache-jena
schema_file: json-schema/fuseki-sparql-api-rdf-term-schema.json
slug: fuseki-sparql-api-rdf-term
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-rdf-term-schema.json\",\n  \"title\": \"RDFTerm\",\n  \"description\": \"An RDF term (URI, literal, or blank node)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"uri\",\n        \"literal\",\n        \"bnode\"\n      ],\n      \"example\": \"uri\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"example\": \"http://example.org/subject\"\n    },\n    \"datatype\": {\n      \"type\": \"string\",\n      \"description\": \"Datatype URI for typed literals\"\n    },\n    \"xml:lang\": {\n      \"type\": \"string\",\n      \"description\": \"Language tag for language-tagged literals\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-rdf-term-schema.json
tags:
- Java
- Linked Data
- OWL
- Ontology
- Open Source
- RDF
- Semantic Web
- SPARQL
title: RDFTerm
---
