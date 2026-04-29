---
description: An object that contains information about a value for a time series property.
layout: schema
name: PropertyValue
properties_list:
- description: ''
  name: timestamp
  type: object
- description: ''
  name: value
  type: object
- description: ''
  name: time
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-value-schema.json
slug: iot-twinmaker-property-value
source_filename: iot-twinmaker-property-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-value-schema.json\",\n  \"title\": \"PropertyValue\",\n  \"description\": \"An object that contains information about a value for a time series property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"The timestamp of a value for a time series property.This field is deprecated and will throw an error in the future. Use time instead.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataValue\"\n        },\n        {\n          \"description\": \"An object that specifies a value for a time series property.\"\n\
  \        }\n      ]\n    },\n    \"time\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"<p>ISO8601 DateTime of a value for a time series property.</p> <p>The time for when the property value was recorded in ISO 8601 format: <i>YYYY-MM-DDThh:mm:ss[.SSSSSSSSS][Z/\\u00b1HH:mm]</i>.</p> <ul> <li> <p> <i>[YYYY]</i>: year</p> </li> <li> <p> <i>[MM]</i>: month</p> </li> <li> <p> <i>[DD]</i>: day</p> </li> <li> <p> <i>[hh]</i>: hour</p> </li> <li> <p> <i>[mm]</i>: minute</p> </li> <li> <p> <i>[ss]</i>: seconds</p> </li> <li> <p> <i>[.SSSSSSSSS]</i>: additional precision, where precedence is maintained. For example: [.573123] is equal to 573123000 nanoseconds.</p> </li> <li> <p> <i>Z</i>: default timezone UTC</p> </li> <li> <p> <i>\\u00b1 HH:mm</i>: time zone offset in Hours and Minutes.</p> </li> </ul> <p> <i>Required sub-fields</i>: YYYY-MM-DDThh:mm:ss and [Z/\\u00b1HH:mm]</p>\"\n        }\n      ]\n \
  \   }\n  },\n  \"required\": [\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-value-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyValue
---
