---
description: Configuration information for port forwarding.
layout: schema
name: PortForwardingConfig
properties_list:
- description: ''
  name: portMappings
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-port-forwarding-config-schema.json
slug: amazon-robomaker-openapi-port-forwarding-config
source_filename: amazon-robomaker-openapi-port-forwarding-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-port-forwarding-config-schema.json\",\n  \"title\": \"PortForwardingConfig\",\n  \"description\": \"Configuration information for port forwarding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortMappingList\"\n        },\n        {\n          \"description\": \"The port mappings for the configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-port-forwarding-config-schema.json
tags:
- Robotics
- Simulation
title: PortForwardingConfig
---
