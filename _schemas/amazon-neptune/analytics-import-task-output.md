---
description: ImportTaskOutput schema from Neptune
layout: schema
name: ImportTaskOutput
properties_list:
- description: ''
  name: graphId
  type: string
- description: ''
  name: taskId
  type: string
- description: ''
  name: source
  type: string
- description: ''
  name: format
  type: string
- description: ''
  name: roleArn
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: importOptions
  type: object
- description: ''
  name: importTaskDetails
  type: object
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/analytics-import-task-output-schema.json
slug: analytics-import-task-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-import-task-output-schema.json\",\n  \"title\": \"ImportTaskOutput\",\n  \"description\": \"ImportTaskOutput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphId\": {\n      \"type\": \"string\"\n    },\n    \"taskId\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"string\"\n    },\n    \"format\": {\n      \"type\": \"string\"\n    },\n    \"roleArn\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INITIALIZING\",\n        \"EXPORTING\",\n        \"ANALYZING_DATA\",\n        \"IMPORTING\",\n        \"REPROVISIONING\",\n        \"ROLLING_BACK\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"CANCELLING\",\n        \"CANCELLED\"\n      ]\n    },\n    \"importOptions\"\
  : {\n      \"type\": \"object\"\n    },\n    \"importTaskDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\"\n        },\n        \"startTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"timeElapsedSeconds\": {\n          \"type\": \"integer\"\n        },\n        \"progressPercentage\": {\n          \"type\": \"integer\"\n        },\n        \"errorCount\": {\n          \"type\": \"integer\"\n        },\n        \"errorDetails\": {\n          \"type\": \"string\"\n        },\n        \"statementCount\": {\n          \"type\": \"integer\"\n        },\n        \"dictionaryEntryCount\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/analytics-import-task-output-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ImportTaskOutput
---
