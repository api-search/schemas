---
description: A workflow run.
layout: schema
name: RunListItem
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: workflowId
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: priority
  type: object
- description: ''
  name: storageCapacity
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
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-run-list-item-schema.json
slug: healthomics-run-list-item
source_filename: healthomics-run-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-run-list-item-schema.json\",\n  \"title\": \"RunListItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunArn\"\n        },\n        {\n          \"description\": \"The run's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunId\"\n        },\n        {\n          \"description\": \"The run's ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunStatus\"\n        },\n        {\n          \"description\": \"The run's status.\"\n        }\n      ]\n    },\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\
  \n        },\n        {\n          \"description\": \"The run's workflow ID.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunName\"\n        },\n        {\n          \"description\": \"The run's name.\"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunListItemPriorityInteger\"\n        },\n        {\n          \"description\": \"The run's priority.\"\n        }\n      ]\n    },\n    \"storageCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunListItemStorageCapacityInteger\"\n        },\n        {\n          \"description\": \"The run's storage capacity.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunTimestamp\"\n        },\n        {\n          \"description\": \"When the run was created.\"\n        }\n     \
  \ ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunTimestamp\"\n        },\n        {\n          \"description\": \"When the run started.\"\n        }\n      ]\n    },\n    \"stopTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunTimestamp\"\n        },\n        {\n          \"description\": \"When the run stopped.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A workflow run.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-run-list-item-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: RunListItem
---
