---
description: StartLoaderJobOutput schema from Neptune
layout: schema
name: StartLoaderJobOutput
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: payload
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-start-loader-job-output-schema.json
slug: data-start-loader-job-output
source_filename: data-start-loader-job-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-start-loader-job-output-schema.json\",\n  \"title\": \"StartLoaderJobOutput\",\n  \"description\": \"StartLoaderJobOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"loadId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the load job.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-start-loader-job-output-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: StartLoaderJobOutput
---
