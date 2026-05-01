---
description: ''
layout: schema
name: GetRunTaskResponse
properties_list:
- description: ''
  name: taskId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: cpus
  type: object
- description: ''
  name: memory
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: stopTime
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: logStream
  type: object
- description: ''
  name: gpus
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-run-task-response-schema.json
slug: healthomics-get-run-task-response
source_filename: healthomics-get-run-task-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-run-task-response-schema.json\",\n  \"title\": \"GetRunTaskResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskId\"\n        },\n        {\n          \"description\": \"The task's ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatus\"\n        },\n        {\n          \"description\": \"The task's status.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskName\"\n        },\n        {\n          \"description\": \"The task's name.\"\n        }\n      ]\n    },\n    \"cpus\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/GetRunTaskResponseCpusInteger\"\n        },\n        {\n          \"description\": \"The task's CPU usage.\"\n        }\n      ]\n    },\n    \"memory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRunTaskResponseMemoryInteger\"\n        },\n        {\n          \"description\": \"The task's memory use in gigabytes.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskTimestamp\"\n        },\n        {\n          \"description\": \"When the task was created.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskTimestamp\"\n        },\n        {\n          \"description\": \"The task's start time.\"\n        }\n      ]\n    },\n    \"stopTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskTimestamp\"\n        },\n        {\n         \
  \ \"description\": \"The task's stop time.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatusMessage\"\n        },\n        {\n          \"description\": \"The task's status message.\"\n        }\n      ]\n    },\n    \"logStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskLogStream\"\n        },\n        {\n          \"description\": \"The task's log stream.\"\n        }\n      ]\n    },\n    \"gpus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRunTaskResponseGpusInteger\"\n        },\n        {\n          \"description\": \" The number of Graphics Processing Units (GPU) specified in the task. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-run-task-response-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetRunTaskResponse
---
