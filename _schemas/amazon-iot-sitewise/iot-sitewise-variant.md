---
description: Contains an asset property value (of a single type only).
layout: schema
name: Variant
properties_list:
- description: ''
  name: stringValue
  type: object
- description: ''
  name: integerValue
  type: object
- description: ''
  name: doubleValue
  type: object
- description: ''
  name: booleanValue
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-variant-schema.json
slug: iot-sitewise-variant
source_filename: iot-sitewise-variant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-variant-schema.json\",\n  \"title\": \"Variant\",\n  \"description\": \"Contains an asset property value (of a single type only).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stringValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyValueStringValue\"\n        },\n        {\n          \"description\": \"Asset property data of type string (sequence of characters).\"\n        }\n      ]\n    },\n    \"integerValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyValueIntegerValue\"\n        },\n        {\n          \"description\": \"Asset property data of type integer (whole number).\"\n        }\n      ]\n    },\n    \"doubleValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyValueDoubleValue\"\
  \n        },\n        {\n          \"description\": \"Asset property data of type double (floating point number).\"\n        }\n      ]\n    },\n    \"booleanValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyValueBooleanValue\"\n        },\n        {\n          \"description\": \"Asset property data of type Boolean (true or false).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-variant-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: Variant
---
