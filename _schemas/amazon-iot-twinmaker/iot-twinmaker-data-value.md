---
description: An object that specifies a value for a property.
layout: schema
name: DataValue
properties_list:
- description: ''
  name: booleanValue
  type: object
- description: ''
  name: doubleValue
  type: object
- description: ''
  name: integerValue
  type: object
- description: ''
  name: longValue
  type: object
- description: ''
  name: stringValue
  type: object
- description: ''
  name: listValue
  type: object
- description: ''
  name: mapValue
  type: object
- description: ''
  name: relationshipValue
  type: object
- description: ''
  name: expression
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-data-value-schema.json
slug: iot-twinmaker-data-value
source_filename: iot-twinmaker-data-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-data-value-schema.json\",\n  \"title\": \"DataValue\",\n  \"description\": \"An object that specifies a value for a property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"booleanValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value.\"\n        }\n      ]\n    },\n    \"doubleValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"A double value.\"\n        }\n      ]\n    },\n    \"integerValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"An integer value.\"\n        }\n      ]\n\
  \    },\n    \"longValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"A long value.\"\n        }\n      ]\n    },\n    \"stringValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A string value.\"\n        }\n      ]\n    },\n    \"listValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataValueList\"\n        },\n        {\n          \"description\": \"A list of multiple values.\"\n        }\n      ]\n    },\n    \"mapValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataValueMap\"\n        },\n        {\n          \"description\": \"An object that maps strings to multiple <code>DataValue</code> objects.\"\n        }\n      ]\n    },\n    \"relationshipValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelationshipValue\"\
  \n        },\n        {\n          \"description\": \"A value that relates a component to another component.\"\n        }\n      ]\n    },\n    \"expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Expression\"\n        },\n        {\n          \"description\": \"An expression that produces the value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-data-value-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: DataValue
---
