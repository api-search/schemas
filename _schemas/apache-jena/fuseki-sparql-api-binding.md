---
description: A single result binding
layout: schema
name: Binding
properties_list:
- description: ''
  name: s
  type: object
- description: ''
  name: p
  type: object
- description: ''
  name: o
  type: object
provider_name: Apache Jena
provider_slug: apache-jena
schema_file: json-schema/fuseki-sparql-api-binding-schema.json
slug: fuseki-sparql-api-binding
source_filename: fuseki-sparql-api-binding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-binding-schema.json\",\n  \"title\": \"Binding\",\n  \"description\": \"A single result binding\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"s\": {\n      \"$ref\": \"#/components/schemas/RDFTerm\"\n    },\n    \"p\": {\n      \"$ref\": \"#/components/schemas/RDFTerm\"\n    },\n    \"o\": {\n      \"$ref\": \"#/components/schemas/RDFTerm\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-binding-schema.json
tags:
- Java
- Linked Data
- OWL
- Ontology
- Open Source
- RDF
- Semantic Web
- SPARQL
title: Binding
---
