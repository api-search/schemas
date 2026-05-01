---
description: UpdateConnectivityInfoResponse schema
layout: schema
name: UpdateConnectivityInfoResponse
properties_list:
- description: ''
  name: version
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-update-connectivity-info-response-schema.json
slug: iot-greengrass-update-connectivity-info-response
source_filename: iot-greengrass-update-connectivity-info-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-update-connectivity-info-response-schema.json\",\n  \"title\": \"UpdateConnectivityInfoResponse\",\n  \"description\": \"UpdateConnectivityInfoResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"Version\"\n          },\n          \"description\": \"The new version of the connectivity information for the core device.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"Message\"\n          },\n          \"description\": \"A message about the connectivity\
  \ information update request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-update-connectivity-info-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: UpdateConnectivityInfoResponse
---
