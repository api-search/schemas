---
description: The input for the <a>StopConfigurationRecorder</a> action.
layout: schema
name: StopConfigurationRecorderRequest
properties_list:
- description: ''
  name: ConfigurationRecorderName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-stop-configuration-recorder-request-schema.json
slug: config-stop-configuration-recorder-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-stop-configuration-recorder-request-schema.json\",\n  \"title\": \"StopConfigurationRecorderRequest\",\n  \"description\": \"The input for the <a>StopConfigurationRecorder</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationRecorderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecorderName\"\n        },\n        {\n          \"description\": \"The name of the recorder object that records each configuration change made to the resources.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationRecorderName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-stop-configuration-recorder-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: StopConfigurationRecorderRequest
---
