---
description: DescribeDimensionResponse schema
layout: schema
name: DescribeDimensionResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: stringValues
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-dimension-response-schema.json
slug: iot-device-defender-describe-dimension-response
source_filename: iot-device-defender-describe-dimension-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-dimension-response-schema.json\",\n  \"title\": \"DescribeDimensionResponse\",\n  \"description\": \"DescribeDimensionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionName\"\n        },\n        {\n          \"description\": \"The unique identifier for the dimension.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the dimension.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionType\"\n        },\n\
  \        {\n          \"description\": \"The type of the dimension.\"\n        }\n      ]\n    },\n    \"stringValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionStringValues\"\n        },\n        {\n          \"description\": \"The value or list of values used to scope the dimension. For example, for topic filters, this is the pattern used to match the MQTT topic name.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the dimension was created.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the dimension was last modified.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-dimension-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeDimensionResponse
---
