---
description: A group of signals that are defined in a hierarchical structure.
layout: schema
name: Branch
properties_list:
- description: ''
  name: fullyQualifiedName
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: deprecationMessage
  type: object
- description: ''
  name: comment
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-branch-schema.json
slug: iot-fleetwise-branch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-branch-schema.json\",\n  \"title\": \"Branch\",\n  \"description\": \"A group of signals that are defined in a hierarchical structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fullyQualifiedName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/string\"\n        },\n        {\n          \"description\": \"The fully qualified name of the branch. For example, the fully qualified name of a branch might be <code>Vehicle.Body.Engine</code>.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"A brief description of the branch.\"\n        }\n      ]\n    },\n    \"deprecationMessage\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/message\"\n        },\n        {\n          \"description\": \"The deprecation message for the node or the branch that was moved or deleted.\"\n        }\n      ]\n    },\n    \"comment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/message\"\n        },\n        {\n          \"description\": \"A comment in addition to the description.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fullyQualifiedName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-branch-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: Branch
---
