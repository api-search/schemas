---
description: ''
layout: schema
name: UpdateWorkflowRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-update-workflow-request-schema.json
slug: healthomics-update-workflow-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-update-workflow-request-schema.json\",\n  \"title\": \"UpdateWorkflowRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowName\"\n        },\n        {\n          \"description\": \"A name for the workflow.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDescription\"\n        },\n        {\n          \"description\": \"A description for the workflow.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-update-workflow-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: UpdateWorkflowRequest
---
