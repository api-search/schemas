---
description: ListImportTasksOutput schema from Neptune
layout: schema
name: ListImportTasksOutput
properties_list:
- description: ''
  name: tasks
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-list-import-tasks-output-schema.json
slug: analytics-list-import-tasks-output
source_filename: analytics-list-import-tasks-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-list-import-tasks-output-schema.json\",\n  \"title\": \"ListImportTasksOutput\",\n  \"description\": \"ListImportTasksOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"graphId\": {\n            \"type\": \"string\"\n          },\n          \"taskId\": {\n            \"type\": \"string\"\n          },\n          \"source\": {\n            \"type\": \"string\"\n          },\n          \"format\": {\n            \"type\": \"string\"\n          },\n          \"roleArn\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"nextToken\"\
  : {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-list-import-tasks-output-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ListImportTasksOutput
---
