---
description: List of Fuseki datasets
layout: schema
name: DatasetList
properties_list:
- description: ''
  name: datasets
  type: array
provider_name: Apache Jena
provider_slug: apache-jena
schema_file: json-schema/fuseki-sparql-api-dataset-list-schema.json
slug: fuseki-sparql-api-dataset-list
source_filename: fuseki-sparql-api-dataset-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-dataset-list-schema.json\",\n  \"title\": \"DatasetList\",\n  \"description\": \"List of Fuseki datasets\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Dataset\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-dataset-list-schema.json
tags:
- Java
- Linked Data
- OWL
- Ontology
- Open Source
- RDF
- Semantic Web
- SPARQL
title: DatasetList
---
