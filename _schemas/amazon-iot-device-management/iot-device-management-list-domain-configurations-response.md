---
description: ListDomainConfigurationsResponse schema
layout: schema
name: ListDomainConfigurationsResponse
properties_list:
- description: ''
  name: domainConfigurations
  type: object
- description: ''
  name: nextMarker
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-list-domain-configurations-response-schema.json
slug: iot-device-management-list-domain-configurations-response
source_filename: iot-device-management-list-domain-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-domain-configurations-response-schema.json\",\n  \"title\": \"ListDomainConfigurationsResponse\",\n  \"description\": \"ListDomainConfigurationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainConfigurations\"\n        },\n        {\n          \"description\": \"A list of objects that contain summary information about the user's domain configurations.\"\n        }\n      ]\n    },\n    \"nextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"The marker for the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-list-domain-configurations-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: ListDomainConfigurationsResponse
---
