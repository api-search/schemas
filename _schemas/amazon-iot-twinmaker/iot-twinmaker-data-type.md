---
description: An object that specifies the data type of a property.
layout: schema
name: DataType
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: nestedType
  type: object
- description: ''
  name: allowedValues
  type: object
- description: ''
  name: unitOfMeasure
  type: object
- description: ''
  name: relationship
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-data-type-schema.json
slug: iot-twinmaker-data-type
source_filename: iot-twinmaker-data-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-data-type-schema.json\",\n  \"title\": \"DataType\",\n  \"description\": \"An object that specifies the data type of a property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n        {\n          \"description\": \"The underlying type of the data type.\"\n        }\n      ]\n    },\n    \"nestedType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataType\"\n        },\n        {\n          \"description\": \"The nested type in the data type.\"\n        }\n      ]\n    },\n    \"allowedValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataValueList\"\n        },\n        {\n          \"description\": \"\
  The allowed values for this data type.\"\n        }\n      ]\n    },\n    \"unitOfMeasure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The unit of measure used in this data type.\"\n        }\n      ]\n    },\n    \"relationship\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Relationship\"\n        },\n        {\n          \"description\": \"A relationship that associates a component with another component.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-data-type-schema.json
tags:
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: DataType
---
