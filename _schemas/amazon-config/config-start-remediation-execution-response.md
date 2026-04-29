---
description: StartRemediationExecutionResponse schema
layout: schema
name: StartRemediationExecutionResponse
properties_list:
- description: ''
  name: FailureMessage
  type: object
- description: ''
  name: FailedItems
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-start-remediation-execution-response-schema.json
slug: config-start-remediation-execution-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-remediation-execution-response-schema.json\",\n  \"title\": \"StartRemediationExecutionResponse\",\n  \"description\": \"StartRemediationExecutionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailureMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Returns a failure message. For example, the resource is already compliant.\"\n        }\n      ]\n    },\n    \"FailedItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceKeys\"\n        },\n        {\n          \"description\": \"For resources that have failed to start execution, the API returns a resource key object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-remediation-execution-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: StartRemediationExecutionResponse
---
