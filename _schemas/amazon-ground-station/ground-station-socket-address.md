---
description: Information about the socket address.
layout: schema
name: SocketAddress
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: port
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-socket-address-schema.json
slug: ground-station-socket-address
source_filename: ground-station-socket-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-socket-address-schema.json\",\n  \"title\": \"SocketAddress\",\n  \"description\": \"Information about the socket address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Name of a socket address.\"\n        }\n      ]\n    },\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Port of a socket address.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"port\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-socket-address-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: SocketAddress
---
