---
description: ListDimensionsResponse schema
layout: schema
name: ListDimensionsResponse
properties_list:
- description: ''
  name: dimensionNames
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-dimensions-response-schema.json
slug: iot-device-defender-list-dimensions-response
source_filename: iot-device-defender-list-dimensions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-dimensions-response-schema.json\",\n  \"title\": \"ListDimensionsResponse\",\n  \"description\": \"ListDimensionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dimensionNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionNames\"\n        },\n        {\n          \"description\": \"A list of the names of the defined dimensions. Use <code>DescribeDimension</code> to get details for a dimension.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that can be used to retrieve the next set of results, or <code>null</code> if there are no additional results.\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-dimensions-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListDimensionsResponse
---
