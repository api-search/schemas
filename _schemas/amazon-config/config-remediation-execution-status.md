---
description: Provides details of the current status of the invoked remediation action for that resource.
layout: schema
name: RemediationExecutionStatus
properties_list:
- description: ''
  name: ResourceKey
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: StepDetails
  type: object
- description: ''
  name: InvocationTime
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-remediation-execution-status-schema.json
slug: config-remediation-execution-status
source_filename: config-remediation-execution-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-execution-status-schema.json\",\n  \"title\": \"RemediationExecutionStatus\",\n  \"description\": \"Provides details of the current status of the invoked remediation action for that resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceKey\": {\n      \"$ref\": \"#/components/schemas/ResourceKey\"\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationExecutionState\"\n        },\n        {\n          \"description\": \"ENUM of the values.\"\n        }\n      ]\n    },\n    \"StepDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationExecutionSteps\"\n        },\n        {\n          \"description\": \"Details of every step.\"\n        }\n      ]\n    },\n    \"InvocationTime\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"Start time when the remediation was executed.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time when the remediation execution was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-remediation-execution-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: RemediationExecutionStatus
---
