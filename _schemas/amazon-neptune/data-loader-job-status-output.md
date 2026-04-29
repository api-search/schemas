---
description: LoaderJobStatusOutput schema from Neptune
layout: schema
name: LoaderJobStatusOutput
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: payload
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-loader-job-status-output-schema.json
slug: data-loader-job-status-output
source_filename: data-loader-job-status-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-loader-job-status-output-schema.json\",\n  \"title\": \"LoaderJobStatusOutput\",\n  \"description\": \"LoaderJobStatusOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"feedCount\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"overallStatus\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"fullUri\": {\n              \"type\": \"string\"\n            },\n            \"runNumber\": {\n              \"type\": \"integer\"\n            },\n            \"retryNumber\": {\n              \"type\": \"integer\"\n            },\n   \
  \         \"status\": {\n              \"type\": \"string\"\n            },\n            \"totalTimeSpent\": {\n              \"type\": \"integer\"\n            },\n            \"startTime\": {\n              \"type\": \"integer\"\n            },\n            \"totalRecords\": {\n              \"type\": \"integer\"\n            },\n            \"totalDuplicates\": {\n              \"type\": \"integer\"\n            },\n            \"parsingErrors\": {\n              \"type\": \"integer\"\n            },\n            \"datatypeMismatchErrors\": {\n              \"type\": \"integer\"\n            },\n            \"insertErrors\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-loader-job-status-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: LoaderJobStatusOutput
---
