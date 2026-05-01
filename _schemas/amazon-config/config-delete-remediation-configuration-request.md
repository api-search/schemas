---
description: DeleteRemediationConfigurationRequest schema
layout: schema
name: DeleteRemediationConfigurationRequest
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: ResourceType
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-remediation-configuration-request-schema.json
slug: config-delete-remediation-configuration-request
source_filename: config-delete-remediation-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-remediation-configuration-request-schema.json\",\n  \"title\": \"DeleteRemediationConfigurationRequest\",\n  \"description\": \"DeleteRemediationConfigurationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of the Config rule for which you want to delete remediation configuration.\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of a resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigRuleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-remediation-configuration-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteRemediationConfigurationRequest
---
