---
description: Data for agent discovery.
layout: schema
name: DiscoveryData
properties_list:
- description: ''
  name: capabilityArns
  type: object
- description: ''
  name: privateIpAddresses
  type: object
- description: ''
  name: publicIpAddresses
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-discovery-data-schema.json
slug: ground-station-discovery-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-discovery-data-schema.json\",\n  \"title\": \"DiscoveryData\",\n  \"description\": \"Data for agent discovery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilityArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapabilityArnList\"\n        },\n        {\n          \"description\": \"List of capabilities to associate with agent.\"\n        }\n      ]\n    },\n    \"privateIpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressList\"\n        },\n        {\n          \"description\": \"List of private IP addresses to associate with agent.\"\n        }\n      ]\n    },\n    \"publicIpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressList\"\n\
  \        },\n        {\n          \"description\": \"List of public IP addresses to associate with agent.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"capabilityArns\",\n    \"privateIpAddresses\",\n    \"publicIpAddresses\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-discovery-data-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: DiscoveryData
---
