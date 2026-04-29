---
description: A general abstraction of a signal. A node can be specified as an actuator, attribute, branch, or sensor.
layout: schema
name: Node
properties_list:
- description: ''
  name: branch
  type: object
- description: <p>An input component that reports the environmental condition of a vehicle.</p> <note> <p>You can collect data about fluid levels, temperatures, vibrations, or battery voltage from sensors.</p> </not
  name: sensor
  type: object
- description: ''
  name: actuator
  type: object
- description: ''
  name: attribute
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-node-schema.json
slug: iot-fleetwise-node
source_filename: iot-fleetwise-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-node-schema.json\",\n  \"title\": \"Node\",\n  \"description\": \"A general abstraction of a signal. A node can be specified as an actuator, attribute, branch, or sensor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Branch\"\n        },\n        {\n          \"description\": \"<p>Information about a node specified as a branch.</p> <note> <p>A group of signals that are defined in a hierarchical structure.</p> </note>\"\n        }\n      ]\n    },\n    \"sensor\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"fullyQualifiedName\",\n        \"dataType\"\n      ],\n      \"properties\": {\n        \"fullyQualifiedName\": {\n          \"allOf\": [\n            {\n         \
  \     \"$ref\": \"#/components/schemas/string\"\n            },\n            {\n              \"description\": \"The fully qualified name of the sensor. For example, the fully qualified name of a sensor might be <code>Vehicle.Body.Engine.Battery</code>.\"\n            }\n          ]\n        },\n        \"dataType\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/NodeDataType\"\n            },\n            {\n              \"description\": \"The specified data type of the sensor. \"\n            }\n          ]\n        },\n        \"description\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/description\"\n            },\n            {\n              \"description\": \"A brief description of a sensor.\"\n            }\n          ]\n        },\n        \"unit\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/string\"\n            },\n            {\n           \
  \   \"description\": \"The scientific unit of measurement for data collected by the sensor.\"\n            }\n          ]\n        },\n        \"allowedValues\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/listOfStrings\"\n            },\n            {\n              \"description\": \"A list of possible values a sensor can take.\"\n            }\n          ]\n        },\n        \"min\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/double\"\n            },\n            {\n              \"description\": \"The specified possible minimum value of the sensor.\"\n            }\n          ]\n        },\n        \"max\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/double\"\n            },\n            {\n              \"description\": \"The specified possible maximum value of the sensor.\"\n            }\n          ]\n        },\n        \"deprecationMessage\"\
  : {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/message\"\n            },\n            {\n              \"description\": \"The deprecation message for the node or the branch that was moved or deleted.\"\n            }\n          ]\n        },\n        \"comment\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/message\"\n            },\n            {\n              \"description\": \"A comment in addition to the description.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"<p>An input component that reports the environmental condition of a vehicle.</p> <note> <p>You can collect data about fluid levels, temperatures, vibrations, or battery voltage from sensors.</p> </note>\"\n    },\n    \"actuator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Actuator\"\n        },\n        {\n          \"description\": \"<p>Information about a node specified\
  \ as an actuator.</p> <note> <p>An actuator is a digital representation of a vehicle device.</p> </note>\"\n        }\n      ]\n    },\n    \"attribute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Attribute\"\n        },\n        {\n          \"description\": \"<p>Information about a node specified as an attribute.</p> <note> <p>An attribute represents static information about a vehicle.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-node-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: Node
---
