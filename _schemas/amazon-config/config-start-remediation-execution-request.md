---
description: StartRemediationExecutionRequest schema
layout: schema
name: StartRemediationExecutionRequest
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: ResourceKeys
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-start-remediation-execution-request-schema.json
slug: config-start-remediation-execution-request
source_filename: config-start-remediation-execution-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-remediation-execution-request-schema.json\",\n  \"title\": \"StartRemediationExecutionRequest\",\n  \"description\": \"StartRemediationExecutionRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The list of names of Config rules that you want to run remediation execution for.\"\n        }\n      ]\n    },\n    \"ResourceKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceKeys\"\n        },\n        {\n          \"description\": \"A list of resource keys to be processed with the current request. Each element in the list consists of the resource type and resource ID. \"\n\
  \        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigRuleName\",\n    \"ResourceKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-remediation-execution-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: StartRemediationExecutionRequest
---
