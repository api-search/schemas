---
description: UpdateConnectivityInfoRequest schema
layout: schema
name: UpdateConnectivityInfoRequest
properties_list:
- description: ''
  name: connectivityInfo
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-update-connectivity-info-request-schema.json
slug: iot-greengrass-update-connectivity-info-request
source_filename: iot-greengrass-update-connectivity-info-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-update-connectivity-info-request-schema.json\",\n  \"title\": \"UpdateConnectivityInfoRequest\",\n  \"description\": \"UpdateConnectivityInfoRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectivityInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/connectivityInfoList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ConnectivityInfo\"\n          },\n          \"description\": \"The connectivity information for the core device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"connectivityInfo\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-update-connectivity-info-request-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: UpdateConnectivityInfoRequest
---
