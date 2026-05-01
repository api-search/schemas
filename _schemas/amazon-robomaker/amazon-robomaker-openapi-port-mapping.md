---
description: An object representing a port mapping.
layout: schema
name: PortMapping
properties_list:
- description: ''
  name: jobPort
  type: object
- description: ''
  name: applicationPort
  type: object
- description: ''
  name: enableOnPublicIp
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-port-mapping-schema.json
slug: amazon-robomaker-openapi-port-mapping
source_filename: amazon-robomaker-openapi-port-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-port-mapping-schema.json\",\n  \"title\": \"PortMapping\",\n  \"description\": \"An object representing a port mapping.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Port\"\n        },\n        {\n          \"description\": \"The port number on the simulation job instance to use as a remote connection point. \"\n        }\n      ]\n    },\n    \"applicationPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonSystemPort\"\n        },\n        {\n          \"description\": \"The port number on the application.\"\n        }\n      ]\n    },\n    \"enableOnPublicIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\
  \n        },\n        {\n          \"description\": \"A Boolean indicating whether to enable this port mapping on public IP.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobPort\",\n    \"applicationPort\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-port-mapping-schema.json
tags:
- Robotics
- Simulation
title: PortMapping
---
