---
description: ListProvisioningTemplatesResponse schema
layout: schema
name: ListProvisioningTemplatesResponse
properties_list:
- description: ''
  name: templates
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-provisioning-templates-response-schema.json
slug: iot-device-management-list-provisioning-templates-response
source_filename: iot-device-management-list-provisioning-templates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-provisioning-templates-response-schema.json\",\n  \"title\": \"ListProvisioningTemplatesResponse\",\n  \"description\": \"ListProvisioningTemplatesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisioningTemplateListing\"\n        },\n        {\n          \"description\": \"A list of provisioning templates\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to retrieve the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-provisioning-templates-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListProvisioningTemplatesResponse
---
