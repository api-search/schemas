---
description: JobStatusResponse schema from Neptune
layout: schema
name: JobStatusResponse
properties_list:
- description: The current status of the job.
  name: status
  type: string
- description: The job identifier.
  name: id
  type: string
- description: ''
  name: processingJob
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/ml-job-status-response-schema.json
slug: ml-job-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-job-status-response-schema.json\",\n  \"title\": \"JobStatusResponse\",\n  \"description\": \"JobStatusResponse schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the job.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The job identifier.\"\n    },\n    \"processingJob\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"arn\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\"\n        },\n        \"outputLocation\": {\n          \"type\": \"string\"\n        },\n        \"failureReason\": {\n          \"type\": \"string\"\n\
  \        },\n        \"cloudwatchLogUrl\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/ml-job-status-response-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: JobStatusResponse
---
