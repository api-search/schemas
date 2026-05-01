---
description: GetPropertyValueResponse schema
layout: schema
name: GetPropertyValueResponse
properties_list:
- description: ''
  name: propertyValues
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: tabularPropertyValues
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-get-property-value-response-schema.json
slug: iot-twinmaker-get-property-value-response
source_filename: iot-twinmaker-get-property-value-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-property-value-response-schema.json\",\n  \"title\": \"GetPropertyValueResponse\",\n  \"description\": \"GetPropertyValueResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"propertyValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyLatestValueMap\"\n        },\n        {\n          \"description\": \"An object that maps strings to the properties and latest property values in the response. Each string in the mapping must be unique to this object.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that specifies the next page of results.\"\n        }\n      ]\n    },\n\
  \    \"tabularPropertyValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TabularPropertyValues\"\n        },\n        {\n          \"description\": \"A table of property values.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-property-value-response-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: GetPropertyValueResponse
---
