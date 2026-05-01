---
description: A workflow parameter.
layout: schema
name: WorkflowParameter
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: optional
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-workflow-parameter-schema.json
slug: healthomics-workflow-parameter
source_filename: healthomics-workflow-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-workflow-parameter-schema.json\",\n  \"title\": \"WorkflowParameter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowParameterDescription\"\n        },\n        {\n          \"description\": \"The parameter's description.\"\n        }\n      ]\n    },\n    \"optional\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the parameter is optional.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A workflow parameter.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-workflow-parameter-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: WorkflowParameter
---
