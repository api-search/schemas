---
description: A signal that represents static information about the vehicle, such as engine type or manufacturing date.
layout: schema
name: Attribute
properties_list:
- description: ''
  name: fullyQualifiedName
  type: object
- description: ''
  name: dataType
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: unit
  type: object
- description: ''
  name: allowedValues
  type: object
- description: ''
  name: min
  type: object
- description: ''
  name: max
  type: object
- description: ''
  name: assignedValue
  type: object
- description: ''
  name: defaultValue
  type: object
- description: ''
  name: deprecationMessage
  type: object
- description: ''
  name: comment
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-attribute-schema.json
slug: iot-fleetwise-attribute
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-attribute-schema.json\",\n  \"title\": \"Attribute\",\n  \"description\": \"A signal that represents static information about the vehicle, such as engine type or manufacturing date.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fullyQualifiedName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The fully qualified name of the attribute. For example, the fully qualified name of an attribute might be <code>Vehicle.Body.Engine.Type</code>.\"\n        }\n      ]\n    },\n    \"dataType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeDataType\"\n        },\n        {\n          \"description\": \"The specified data type of the attribute. \"\n        }\n\
  \      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"A brief description of the attribute.\"\n        }\n      ]\n    },\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The scientific unit for the attribute.\"\n        }\n      ]\n    },\n    \"allowedValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/listOfStrings\"\n        },\n        {\n          \"description\": \"A list of possible values an attribute can be assigned.\"\n        }\n      ]\n    },\n    \"min\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The specified possible minimum value of the attribute.\"\n        }\n      ]\n    },\n    \"max\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The specified possible maximum value of the attribute.\"\n        }\n      ]\n    },\n    \"assignedValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"A specified value for the attribute.assignedValue is no longer in use\"\n        }\n      ]\n    },\n    \"defaultValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The default value of the attribute.\"\n        }\n      ]\n    },\n    \"deprecationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/message\"\n        },\n        {\n          \"description\": \"The deprecation message for the node or the branch that was moved or deleted.\"\n        }\n      ]\n\
  \    },\n    \"comment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/message\"\n        },\n        {\n          \"description\": \"A comment in addition to the description.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fullyQualifiedName\",\n    \"dataType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-attribute-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: Attribute
---
