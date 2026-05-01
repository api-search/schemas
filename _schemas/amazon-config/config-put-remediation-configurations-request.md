---
description: PutRemediationConfigurationsRequest schema
layout: schema
name: PutRemediationConfigurationsRequest
properties_list:
- description: ''
  name: RemediationConfigurations
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-remediation-configurations-request-schema.json
slug: config-put-remediation-configurations-request
source_filename: config-put-remediation-configurations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-remediation-configurations-request-schema.json\",\n  \"title\": \"PutRemediationConfigurationsRequest\",\n  \"description\": \"PutRemediationConfigurationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RemediationConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationConfigurations\"\n        },\n        {\n          \"description\": \"A list of remediation configuration objects.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RemediationConfigurations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-remediation-configurations-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutRemediationConfigurationsRequest
---
