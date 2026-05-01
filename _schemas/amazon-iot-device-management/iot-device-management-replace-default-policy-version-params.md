---
description: Parameters to define a mitigation action that adds a blank policy to restrict permissions.
layout: schema
name: ReplaceDefaultPolicyVersionParams
properties_list:
- description: ''
  name: templateName
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-replace-default-policy-version-params-schema.json
slug: iot-device-management-replace-default-policy-version-params
source_filename: iot-device-management-replace-default-policy-version-params-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-replace-default-policy-version-params-schema.json\",\n  \"title\": \"ReplaceDefaultPolicyVersionParams\",\n  \"description\": \"Parameters to define a mitigation action that adds a blank policy to restrict permissions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyTemplateName\"\n        },\n        {\n          \"description\": \"The name of the template to be applied. The only supported value is <code>BLANK_POLICY</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"templateName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-replace-default-policy-version-params-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ReplaceDefaultPolicyVersionParams
---
