---
description: CreateGraphUsingImportTaskInput schema from Neptune
layout: schema
name: CreateGraphUsingImportTaskInput
properties_list:
- description: The name of the graph to create.
  name: graphName
  type: string
- description: S3 URI of the source data to import.
  name: source
  type: string
- description: IAM role ARN with S3 access.
  name: roleArn
  type: string
- description: ''
  name: provisionedMemory
  type: integer
- description: The format of the source data.
  name: format
  type: string
- description: ''
  name: tags
  type: object
- description: ''
  name: deletionProtection
  type: boolean
- description: ''
  name: publicConnectivity
  type: boolean
- description: ''
  name: kmsKeyIdentifier
  type: string
- description: ''
  name: vectorSearchConfiguration
  type: object
- description: ''
  name: replicaCount
  type: integer
- description: Additional import configuration options.
  name: importOptions
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-create-graph-using-import-task-input-schema.json
slug: analytics-create-graph-using-import-task-input
source_filename: analytics-create-graph-using-import-task-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-create-graph-using-import-task-input-schema.json\",\n  \"title\": \"CreateGraphUsingImportTaskInput\",\n  \"description\": \"CreateGraphUsingImportTaskInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the graph to create.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"S3 URI of the source data to import.\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\",\n      \"description\": \"IAM role ARN with S3 access.\"\n    },\n    \"provisionedMemory\": {\n      \"type\": \"integer\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The format of the source data.\",\n      \"enum\": [\n        \"CSV\",\n        \"\
  OPEN_CYPHER\",\n        \"PARQUET\",\n        \"NTRIPLES\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"deletionProtection\": {\n      \"type\": \"boolean\"\n    },\n    \"publicConnectivity\": {\n      \"type\": \"boolean\"\n    },\n    \"kmsKeyIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"vectorSearchConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dimension\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"replicaCount\": {\n      \"type\": \"integer\"\n    },\n    \"importOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Additional import configuration options.\"\n    }\n  },\n  \"required\": [\n    \"graphName\",\n    \"source\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-create-graph-using-import-task-input-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateGraphUsingImportTaskInput
---
