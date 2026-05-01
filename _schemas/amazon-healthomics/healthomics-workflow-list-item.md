---
description: A workflow.
layout: schema
name: WorkflowListItem
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: digest
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-workflow-list-item-schema.json
slug: healthomics-workflow-list-item
source_filename: healthomics-workflow-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-workflow-list-item-schema.json\",\n  \"title\": \"WorkflowListItem\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowArn\"\n        },\n        {\n          \"description\": \"The workflow's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The workflow's ID.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowName\"\n        },\n        {\n          \"description\": \"The workflow's name.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/WorkflowStatus\"\n        },\n        {\n          \"description\": \"The workflow's status.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The workflow's type.\"\n        }\n      ]\n    },\n    \"digest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDigest\"\n        },\n        {\n          \"description\": \"The workflow's digest.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowTimestamp\"\n        },\n        {\n          \"description\": \"When the workflow was created.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowMetadata\"\n        },\n        {\n          \"description\": \" Any metadata\
  \ available for workflow. The information listed may vary depending on the workflow, and there may also be no metadata to return. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"A workflow.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-workflow-list-item-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: WorkflowListItem
---
