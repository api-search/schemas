---
description: Nodes schema
layout: schema
name: Nodes
properties_list: []
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-nodes-schema.json
slug: iot-fleetwise-nodes
source_filename: iot-fleetwise-nodes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-nodes-schema.json\",\n  \"title\": \"Nodes\",\n  \"description\": \"Nodes schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"branch\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Branch\"\n          },\n          {\n            \"description\": \"<p>Information about a node specified as a branch.</p> <note> <p>A group of signals that are defined in a hierarchical structure.</p> </note>\"\n          }\n        ]\n      },\n      \"sensor\": {\n        \"$ref\": \"#/components/schemas/Sensor\"\n      },\n      \"actuator\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Actuator\"\n          },\n          {\n            \"description\": \"<p>Information about\
  \ a node specified as an actuator.</p> <note> <p>An actuator is a digital representation of a vehicle device.</p> </note>\"\n          }\n        ]\n      },\n      \"attribute\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Attribute\"\n          },\n          {\n            \"description\": \"<p>Information about a node specified as an attribute.</p> <note> <p>An attribute represents static information about a vehicle.</p> </note>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A general abstraction of a signal. A node can be specified as an actuator, attribute, branch, or sensor.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-nodes-schema.json
tags:
- Automotive
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: Nodes
---
