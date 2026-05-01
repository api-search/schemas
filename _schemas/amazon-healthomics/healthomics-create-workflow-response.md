---
description: ''
layout: schema
name: CreateWorkflowResponse
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
  name: tags
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-workflow-response-schema.json
slug: healthomics-create-workflow-response
source_filename: healthomics-create-workflow-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-workflow-response-schema.json\",\n  \"title\": \"CreateWorkflowResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowArn\"\n        },\n        {\n          \"description\": \"The workflow's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The workflow's ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStatus\"\n        },\n        {\n          \"description\": \"The workflow's status.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The workflow's tags.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-workflow-response-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateWorkflowResponse
---
