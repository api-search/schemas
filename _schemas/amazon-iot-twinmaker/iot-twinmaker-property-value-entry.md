---
description: An object that specifies information about time series property values. This object is used and consumed by the <a href="https://docs.aws.amazon.com/iot-twinmaker/latest/apireference/API_BatchPutPropertyValues.html">BatchPutPropertyValues</a> action.
layout: schema
name: PropertyValueEntry
properties_list:
- description: ''
  name: entityPropertyReference
  type: object
- description: ''
  name: propertyValues
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-property-value-entry-schema.json
slug: iot-twinmaker-property-value-entry
source_filename: iot-twinmaker-property-value-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-value-entry-schema.json\",\n  \"title\": \"PropertyValueEntry\",\n  \"description\": \"An object that specifies information about time series property values. This object is used and consumed by the <a href=\\\"https://docs.aws.amazon.com/iot-twinmaker/latest/apireference/API_BatchPutPropertyValues.html\\\">BatchPutPropertyValues</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entityPropertyReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityPropertyReference\"\n        },\n        {\n          \"description\": \"An object that contains information about the entity that has the property.\"\n        }\n      ]\n    },\n    \"propertyValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyValues\"\
  \n        },\n        {\n          \"description\": \"A list of objects that specify time series property values.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"entityPropertyReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-property-value-entry-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: PropertyValueEntry
---
