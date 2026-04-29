---
description: <p>An input component that reports the environmental condition of a vehicle.</p> <note> <p>You can collect data about fluid levels, temperatures, vibrations, or battery voltage from sensors.</p> </note>
layout: schema
name: Sensor
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
  name: deprecationMessage
  type: object
- description: ''
  name: comment
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-sensor-schema.json
slug: iot-fleetwise-sensor
source_filename: iot-fleetwise-sensor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-sensor-schema.json\",\n  \"title\": \"Sensor\",\n  \"description\": \"<p>An input component that reports the environmental condition of a vehicle.</p> <note> <p>You can collect data about fluid levels, temperatures, vibrations, or battery voltage from sensors.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fullyQualifiedName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The fully qualified name of the sensor. For example, the fully qualified name of a sensor might be <code>Vehicle.Body.Engine.Battery</code>.\"\n        }\n      ]\n    },\n    \"dataType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeDataType\"\n        },\n        {\n\
  \          \"description\": \"The specified data type of the sensor. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"A brief description of a sensor.\"\n        }\n      ]\n    },\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The scientific unit of measurement for data collected by the sensor.\"\n        }\n      ]\n    },\n    \"allowedValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/listOfStrings\"\n        },\n        {\n          \"description\": \"A list of possible values a sensor can take.\"\n        }\n      ]\n    },\n    \"min\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The specified possible\
  \ minimum value of the sensor.\"\n        }\n      ]\n    },\n    \"max\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/double\"\n        },\n        {\n          \"description\": \"The specified possible maximum value of the sensor.\"\n        }\n      ]\n    },\n    \"deprecationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/message\"\n        },\n        {\n          \"description\": \"The deprecation message for the node or the branch that was moved or deleted.\"\n        }\n      ]\n    },\n    \"comment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/message\"\n        },\n        {\n          \"description\": \"A comment in addition to the description.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fullyQualifiedName\",\n    \"dataType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-sensor-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: Sensor
---
