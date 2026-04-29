---
description: Request to create a dataset
layout: schema
name: DatasetRequest
properties_list:
- description: Dataset name
  name: dbName
  type: string
- description: Dataset type
  name: dbType
  type: string
provider_name: Apache Jena
provider_slug: apache-jena
schema_file: json-schema/fuseki-sparql-api-dataset-request-schema.json
slug: fuseki-sparql-api-dataset-request
source_filename: fuseki-sparql-api-dataset-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-dataset-request-schema.json\",\n  \"title\": \"DatasetRequest\",\n  \"description\": \"Request to create a dataset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dbName\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset name\",\n      \"example\": \"ds\"\n    },\n    \"dbType\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset type\",\n      \"enum\": [\n        \"tdb\",\n        \"tdb2\",\n        \"mem\"\n      ],\n      \"example\": \"tdb2\"\n    }\n  },\n  \"required\": [\n    \"dbName\",\n    \"dbType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-jena/refs/heads/main/json-schema/fuseki-sparql-api-dataset-request-schema.json
tags:
- Java
- Linked Data
- OWL
- Ontology
- Open Source
- RDF
- Semantic Web
- SPARQL
title: DatasetRequest
---
