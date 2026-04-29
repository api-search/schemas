---
description: GetIndexingConfigurationResponse schema
layout: schema
name: GetIndexingConfigurationResponse
properties_list:
- description: ''
  name: thingIndexingConfiguration
  type: object
- description: ''
  name: thingGroupIndexingConfiguration
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-get-indexing-configuration-response-schema.json
slug: iot-device-defender-get-indexing-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-indexing-configuration-response-schema.json\",\n  \"title\": \"GetIndexingConfigurationResponse\",\n  \"description\": \"GetIndexingConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingIndexingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingIndexingConfiguration\"\n        },\n        {\n          \"description\": \"Thing indexing configuration.\"\n        }\n      ]\n    },\n    \"thingGroupIndexingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingGroupIndexingConfiguration\"\n        },\n        {\n          \"description\": \"The index configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-indexing-configuration-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: GetIndexingConfigurationResponse
---
