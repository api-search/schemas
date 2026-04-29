---
description: The request object for the <code>DeleteConfigurationRecorder</code> action.
layout: schema
name: DeleteConfigurationRecorderRequest
properties_list:
- description: ''
  name: ConfigurationRecorderName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-configuration-recorder-request-schema.json
slug: config-delete-configuration-recorder-request
source_filename: config-delete-configuration-recorder-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-configuration-recorder-request-schema.json\",\n  \"title\": \"DeleteConfigurationRecorderRequest\",\n  \"description\": \"The request object for the <code>DeleteConfigurationRecorder</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationRecorderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecorderName\"\n        },\n        {\n          \"description\": \"The name of the configuration recorder to be deleted. You can retrieve the name of your configuration recorder by using the <code>DescribeConfigurationRecorders</code> action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationRecorderName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-configuration-recorder-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteConfigurationRecorderRequest
---
