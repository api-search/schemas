---
description: <p>A signal that represents a vehicle device such as the engine, heater, and door locks. Data from an actuator reports the state of a certain vehicle device.</p> <note> <p> Updating actuator data can change the state of a device. For example, you can turn on or off the heater by updating its actuator data.</p> </note>
layout: schema
name: Actuator
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
  name: deprecationMessage
  type: object
- description: ''
  name: comment
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-actuator-schema.json
slug: iot-fleetwise-actuator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-actuator-schema.json\",\n  \"title\": \"Actuator\",\n  \"description\": \"<p>A signal that represents a vehicle device such as the engine, heater, and door locks. Data from an actuator reports the state of a certain vehicle device.</p> <note> <p> Updating actuator data can change the state of a device. For example, you can turn on or off the heater by updating its actuator data.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fullyQualifiedName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The fully qualified name of the actuator. For example, the fully qualified name of an actuator might be <code>Vehicle.Front.Left.Door.Lock</code>.\"\n        }\n      ]\n    },\n    \"\
  dataType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeDataType\"\n        },\n        {\n          \"description\": \"The specified data type of the actuator. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"A brief description of the actuator.\"\n        }\n      ]\n    },\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The scientific unit for the actuator.\"\n        }\n      ]\n    },\n    \"allowedValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/listOfStrings\"\n        },\n        {\n          \"description\": \"A list of possible values an actuator can take.\"\n        }\n      ]\n    },\n    \"min\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The specified possible minimum value of an actuator.\"\n        }\n      ]\n    },\n    \"max\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The specified possible maximum value of an actuator.\"\n        }\n      ]\n    },\n    \"assignedValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"A specified value for the actuator.assignedValue is no longer in use\"\n        }\n      ]\n    },\n    \"deprecationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/message\"\n        },\n        {\n          \"description\": \"The deprecation message for the node or the branch that was moved or deleted.\"\n        }\n      ]\n    },\n    \"comment\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/message\"\n        },\n        {\n          \"description\": \"A comment in addition to the description.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fullyQualifiedName\",\n    \"dataType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-actuator-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: Actuator
---
