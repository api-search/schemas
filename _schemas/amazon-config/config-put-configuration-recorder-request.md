---
description: The input for the <a>PutConfigurationRecorder</a> action.
layout: schema
name: PutConfigurationRecorderRequest
properties_list:
- description: ''
  name: ConfigurationRecorder
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-configuration-recorder-request-schema.json
slug: config-put-configuration-recorder-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-configuration-recorder-request-schema.json\",\n  \"title\": \"PutConfigurationRecorderRequest\",\n  \"description\": \"The input for the <a>PutConfigurationRecorder</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationRecorder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRecorder\"\n        },\n        {\n          \"description\": \"An object for the configuration recorder to record configuration changes for specified resource types.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationRecorder\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-configuration-recorder-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutConfigurationRecorderRequest
---
