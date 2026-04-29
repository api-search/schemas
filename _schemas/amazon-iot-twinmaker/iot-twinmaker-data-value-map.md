---
description: DataValueMap schema
layout: schema
name: DataValueMap
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-data-value-map-schema.json
slug: iot-twinmaker-data-value-map
source_filename: iot-twinmaker-data-value-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-data-value-map-schema.json\",\n  \"title\": \"DataValueMap\",\n  \"description\": \"DataValueMap schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"booleanValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Boolean\"\n          },\n          {\n            \"description\": \"A Boolean value.\"\n          }\n        ]\n      },\n      \"doubleValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Double\"\n          },\n          {\n            \"description\": \"A double value.\"\n          }\n        ]\n      },\n      \"integerValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Integer\"\n    \
  \      },\n          {\n            \"description\": \"An integer value.\"\n          }\n        ]\n      },\n      \"longValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Long\"\n          },\n          {\n            \"description\": \"A long value.\"\n          }\n        ]\n      },\n      \"stringValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/String\"\n          },\n          {\n            \"description\": \"A string value.\"\n          }\n        ]\n      },\n      \"listValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DataValueList\"\n          },\n          {\n            \"description\": \"A list of multiple values.\"\n          }\n        ]\n      },\n      \"mapValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DataValueMap\"\n          },\n          {\n            \"description\": \"An object that maps strings\
  \ to multiple <code>DataValue</code> objects.\"\n          }\n        ]\n      },\n      \"relationshipValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RelationshipValue\"\n          },\n          {\n            \"description\": \"A value that relates a component to another component.\"\n          }\n        ]\n      },\n      \"expression\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Expression\"\n          },\n          {\n            \"description\": \"An expression that produces the value.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that specifies a value for a property.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-data-value-map-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: DataValueMap
---
