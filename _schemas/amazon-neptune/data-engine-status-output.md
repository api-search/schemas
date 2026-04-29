---
description: EngineStatusOutput schema from Neptune
layout: schema
name: EngineStatusOutput
properties_list:
- description: The status of the Neptune engine (healthy, recovery, etc.).
  name: status
  type: string
- description: The start time of the engine.
  name: startTime
  type: string
- description: The Neptune engine version.
  name: dbEngineVersion
  type: string
- description: The cluster role (writer or reader).
  name: role
  type: string
- description: The DFE query engine status (enabled or viaQueryHint).
  name: dfeQueryEngine
  type: string
- description: ''
  name: gremlin
  type: object
- description: ''
  name: sparql
  type: object
- description: ''
  name: opencypher
  type: object
- description: ''
  name: labMode
  type: object
- description: ''
  name: features
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-engine-status-output-schema.json
slug: data-engine-status-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-engine-status-output-schema.json\",\n  \"title\": \"EngineStatusOutput\",\n  \"description\": \"EngineStatusOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the Neptune engine (healthy, recovery, etc.).\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"The start time of the engine.\"\n    },\n    \"dbEngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The Neptune engine version.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster role (writer or reader).\"\n    },\n    \"dfeQueryEngine\": {\n      \"type\": \"string\",\n      \"description\": \"The DFE query engine status (enabled or viaQueryHint).\"\
  \n    },\n    \"gremlin\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"sparql\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"opencypher\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"labMode\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"features\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-engine-status-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: EngineStatusOutput
---
