---
description: A workflow run task.
layout: schema
name: TaskListItem
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
  name: gpus
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-task-list-item-schema.json
slug: healthomics-task-list-item
source_filename: healthomics-task-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-task-list-item-schema.json\",\n  \"title\": \"TaskListItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"taskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskId\"\n        },\n        {\n          \"description\": \"The task's ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStatus\"\n        },\n        {\n          \"description\": \"The task's status.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskName\"\n        },\n        {\n          \"description\": \"The task's name.\"\n        }\n      ]\n    },\n    \"cpus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskListItemCpusInteger\"\
  \n        },\n        {\n          \"description\": \"The task's CPU count.\"\n        }\n      ]\n    },\n    \"memory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskListItemMemoryInteger\"\n        },\n        {\n          \"description\": \"The task's memory use in gigabyes.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskTimestamp\"\n        },\n        {\n          \"description\": \"When the task was created.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskTimestamp\"\n        },\n        {\n          \"description\": \"When the task started.\"\n        }\n      ]\n    },\n    \"stopTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskTimestamp\"\n        },\n        {\n          \"description\": \"When the task stopped.\"\n        }\n      ]\n\
  \    },\n    \"gpus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskListItemGpusInteger\"\n        },\n        {\n          \"description\": \" The number of Graphics Processing Units (GPU) specified for the task. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"A workflow run task.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-task-list-item-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: TaskListItem
---
