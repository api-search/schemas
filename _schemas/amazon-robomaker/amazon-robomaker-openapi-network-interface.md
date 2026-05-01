---
description: Describes a network interface.
layout: schema
name: NetworkInterface
properties_list:
- description: ''
  name: networkInterfaceId
  type: object
- description: ''
  name: privateIpAddress
  type: object
- description: ''
  name: publicIpAddress
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-network-interface-schema.json
slug: amazon-robomaker-openapi-network-interface
source_filename: amazon-robomaker-openapi-network-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-network-interface-schema.json\",\n  \"title\": \"NetworkInterface\",\n  \"description\": \"Describes a network interface.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkInterfaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The ID of the network interface.\"\n        }\n      ]\n    },\n    \"privateIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The IPv4 address of the network interface within the subnet.\"\n        }\n      ]\n    },\n    \"publicIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\
  \n        },\n        {\n          \"description\": \"The IPv4 public address of the network interface.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-network-interface-schema.json
tags:
- Robotics
- Simulation
title: NetworkInterface
---
