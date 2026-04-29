---
description: A Fuseki dataset
layout: schema
name: Dataset
properties_list:
- description: Dataset name
  name: ds.name
  type: string
- description: Whether the dataset is active
  name: ds.state
  type: boolean
- description: Available services for this dataset
  name: ds.services
  type: array
provider_name: Apache Jena
provider_slug: apache-jena
schema_file: json-schema/fuseki-sparql-api-dataset-schema.json
slug: fuseki-sparql-api-dataset
source_filename: fuseki-sparql-api-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-dataset-schema.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"A Fuseki dataset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ds.name\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset name\",\n      \"example\": \"/ds\"\n    },\n    \"ds.state\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dataset is active\",\n      \"example\": true\n    },\n    \"ds.services\": {\n      \"type\": \"array\",\n      \"description\": \"Available services for this dataset\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-dataset-schema.json
tags:
- Java
- Linked Data
- OWL
- Ontology
- Open Source
- RDF
- Semantic Web
- SPARQL
title: Dataset
---
