---
description: Ingress address of AgentEndpoint with a port range and an optional mtu.
layout: schema
name: RangedConnectionDetails
properties_list:
- description: ''
  name: mtu
  type: object
- description: ''
  name: socketAddress
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-ranged-connection-details-schema.json
slug: ground-station-ranged-connection-details
source_filename: ground-station-ranged-connection-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ranged-connection-details-schema.json\",\n  \"title\": \"RangedConnectionDetails\",\n  \"description\": \"Ingress address of AgentEndpoint with a port range and an optional mtu.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mtu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RangedConnectionDetailsMtuInteger\"\n        },\n        {\n          \"description\": \"Maximum transmission unit (MTU) size in bytes of a dataflow endpoint.\"\n        }\n      ]\n    },\n    \"socketAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RangedSocketAddress\"\n        },\n        {\n          \"description\": \"A ranged socket address.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"socketAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ranged-connection-details-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: RangedConnectionDetails
---
