---
description: ServiceConnection schema from Palo Alto Networks Prisma Access Configuration API
layout: schema
name: ServiceConnection
properties_list:
- description: Unique identifier for the service connection.
  name: id
  type: string
- description: Name of the service connection.
  name: name
  type: string
- description: Prisma Access compute region.
  name: region
  type: string
- description: Name of the associated IPSec tunnel.
  name: ipsec_tunnel
  type: string
- description: Internal subnets accessible through this connection.
  name: subnets
  type: array
- description: NAT pool CIDR for source translation.
  name: nat_pool
  type: string
- description: Whether QoS is enabled on this connection.
  name: qos_enabled
  type: boolean
- description: ''
  name: folder
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-api-service-connection-schema.json
slug: prisma-access-api-service-connection
source_filename: prisma-access-api-service-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceConnection\",\n  \"description\": \"ServiceConnection schema from Palo Alto Networks Prisma Access Configuration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-service-connection-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the service connection.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the service connection.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Prisma Access compute region.\"\n    },\n    \"ipsec_tunnel\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the associated IPSec tunnel.\"\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      },\n      \"description\": \"Internal subnets accessible through this connection.\"\n    },\n    \"nat_pool\": {\n      \"type\": \"string\",\n      \"description\": \"NAT pool CIDR for source translation.\"\n    },\n    \"qos_enabled\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether QoS is enabled on this connection.\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"region\",\n    \"ipsec_tunnel\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-service-connection-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ServiceConnection
---
