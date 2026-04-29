---
description: A CloudStack network resource providing connectivity for virtual machines.
layout: schema
name: Network
properties_list:
- description: UUID of the network.
  name: id
  type: string
- description: Display name of the network.
  name: name
  type: string
- description: Current state of the network.
  name: state
  type: string
- description: UUID of the zone containing the network.
  name: zoneid
  type: string
- description: Type of network (Isolated, Shared, L2).
  name: type
  type: string
- description: CIDR block of the network.
  name: cidr
  type: string
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-network-schema.json
slug: cloudstack-api-network
source_filename: cloudstack-api-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-network-schema.json\",\n  \"title\": \"Network\",\n  \"description\": \"A CloudStack network resource providing connectivity for virtual machines.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"UUID of the network.\", \"example\": \"net-uuid-1234\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Display name of the network.\", \"example\": \"default-network\" },\n    \"state\": { \"type\": \"string\", \"description\": \"Current state of the network.\", \"example\": \"Implemented\" },\n    \"zoneid\": { \"type\": \"string\", \"description\": \"UUID of the zone containing the network.\", \"example\": \"zone-uuid-abcd\" },\n    \"type\": { \"type\": \"string\", \"description\": \"Type of network (Isolated, Shared, L2).\"\
  , \"example\": \"Isolated\" },\n    \"cidr\": { \"type\": \"string\", \"description\": \"CIDR block of the network.\", \"example\": \"10.0.0.0/24\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-network-schema.json
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: Network
---
