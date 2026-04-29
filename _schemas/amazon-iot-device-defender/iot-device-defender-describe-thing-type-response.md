---
description: The output for the DescribeThingType operation.
layout: schema
name: DescribeThingTypeResponse
properties_list:
- description: ''
  name: thingTypeName
  type: object
- description: ''
  name: thingTypeId
  type: object
- description: ''
  name: thingTypeArn
  type: object
- description: ''
  name: thingTypeProperties
  type: object
- description: ''
  name: thingTypeMetadata
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-thing-type-response-schema.json
slug: iot-device-defender-describe-thing-type-response
source_filename: iot-device-defender-describe-thing-type-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-thing-type-response-schema.json\",\n  \"title\": \"DescribeThingTypeResponse\",\n  \"description\": \"The output for the DescribeThingType operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thingTypeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeName\"\n        },\n        {\n          \"description\": \"The name of the thing type.\"\n        }\n      ]\n    },\n    \"thingTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeId\"\n        },\n        {\n          \"description\": \"The thing type ID.\"\n        }\n      ]\n    },\n    \"thingTypeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeArn\"\n        },\n  \
  \      {\n          \"description\": \"The thing type ARN.\"\n        }\n      ]\n    },\n    \"thingTypeProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeProperties\"\n        },\n        {\n          \"description\": \"The ThingTypeProperties contains information about the thing type including description, and a list of searchable thing attribute names.\"\n        }\n      ]\n    },\n    \"thingTypeMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThingTypeMetadata\"\n        },\n        {\n          \"description\": \"The ThingTypeMetadata contains additional information about the thing type including: creation date and time, a value indicating whether the thing type is deprecated, and a date and time when it was deprecated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-thing-type-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeThingTypeResponse
---
