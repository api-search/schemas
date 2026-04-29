---
description: Name of the step from the SSM document.
layout: schema
name: RemediationExecutionStep
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: StopTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-remediation-execution-step-schema.json
slug: config-remediation-execution-step
source_filename: config-remediation-execution-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-execution-step-schema.json\",\n  \"title\": \"RemediationExecutionStep\",\n  \"description\": \"Name of the step from the SSM document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The details of the step.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationExecutionStepState\"\n        },\n        {\n          \"description\": \"The valid status of the step.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An\
  \ error message if the step was interrupted during execution.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when the step started.\"\n        }\n      ]\n    },\n    \"StopTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when the step stopped.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-execution-step-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: RemediationExecutionStep
---
