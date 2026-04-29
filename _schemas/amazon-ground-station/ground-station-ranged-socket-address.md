---
description: A socket address with a port range.
layout: schema
name: RangedSocketAddress
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: portRange
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-ranged-socket-address-schema.json
slug: ground-station-ranged-socket-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ranged-socket-address-schema.json\",\n  \"title\": \"RangedSocketAddress\",\n  \"description\": \"A socket address with a port range.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpV4Address\"\n        },\n        {\n          \"description\": \"IPv4 socket address.\"\n        }\n      ]\n    },\n    \"portRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerRange\"\n        },\n        {\n          \"description\": \"Port range of a socket address.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"portRange\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ranged-socket-address-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: RangedSocketAddress
---
