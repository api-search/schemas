---
description: MLJobStatusOutput schema from Neptune
layout: schema
name: MLJobStatusOutput
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: processingJob
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-ml-job-status-output-schema.json
slug: data-ml-job-status-output
source_filename: data-ml-job-status-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-ml-job-status-output-schema.json\",\n  \"title\": \"MLJobStatusOutput\",\n  \"description\": \"MLJobStatusOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"processingJob\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"arn\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        },\n        \"outputLocation\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-ml-job-status-output-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: MLJobStatusOutput
---
