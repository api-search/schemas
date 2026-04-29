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
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-list-provisioning-templates-response-schema.json
slug: iot-core-list-provisioning-templates-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-provisioning-templates-response-schema.json\",\n  \"title\": \"ListProvisioningTemplatesResponse\",\n  \"description\": \"ListProvisioningTemplatesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisioningTemplateListing\"\n        },\n        {\n          \"description\": \"A list of provisioning templates\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to retrieve the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-list-provisioning-templates-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: ListProvisioningTemplatesResponse
---
