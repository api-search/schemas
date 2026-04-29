---
description: Egress address of AgentEndpoint with an optional mtu.
layout: schema
name: ConnectionDetails
properties_list:
- description: ''
  name: mtu
  type: object
- description: ''
  name: socketAddress
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-connection-details-schema.json
slug: ground-station-connection-details
source_filename: ground-station-connection-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-connection-details-schema.json\",\n  \"title\": \"ConnectionDetails\",\n  \"description\": \"Egress address of AgentEndpoint with an optional mtu.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mtu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"Maximum transmission unit (MTU) size in bytes of a dataflow endpoint.\"\n        }\n      ]\n    },\n    \"socketAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SocketAddress\"\n        },\n        {\n          \"description\": \"A socket address.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"socketAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-connection-details-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ConnectionDetails
---
