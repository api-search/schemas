---
description: RemoteNetwork schema from Palo Alto Networks SASE Configuration Orchestration API
layout: schema
name: RemoteNetwork
properties_list:
- description: Unique identifier of the remote network.
  name: id
  type: string
- description: Display name of the remote network.
  name: name
  type: string
- description: Description of the remote network's location or purpose.
  name: description
  type: string
- description: Prisma Access gateway location for this tunnel.
  name: location
  type: string
- description: Network subnets at the remote site (CIDR notation).
  name: subnets
  type: array
- description: ''
  name: ike_gateway
  type: object
- description: ''
  name: ipsec_tunnel
  type: object
- description: Current IPsec tunnel connection status.
  name: tunnel_status
  type: string
- description: Allocated bandwidth in Mbps for this remote network.
  name: bandwidth_mbps
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-config-orchestration-api-remote-network-schema.json
slug: sase-config-orchestration-api-remote-network
source_filename: sase-config-orchestration-api-remote-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RemoteNetwork\",\n  \"description\": \"RemoteNetwork schema from Palo Alto Networks SASE Configuration Orchestration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-remote-network-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the remote network.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the remote network.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the remote network's location or purpose.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Prisma Access gateway location for this tunnel.\"\n    },\n    \"subnets\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Network subnets at the remote site (CIDR notation).\"\n    },\n    \"ike_gateway\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"peer_ip\": {\n          \"type\": \"string\",\n          \"description\": \"Public IP address of the remote peer gateway.\"\n        },\n        \"peer_id\": {\n          \"type\": \"string\",\n          \"description\": \"IKE peer identity.\"\n        },\n        \"local_ip\": {\n          \"type\": \"string\",\n          \"description\": \"Prisma Access local IKE gateway IP address.\"\n        },\n        \"ike_version\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"IKEv1\",\n            \"IKEv2\"\n          ],\n          \"description\": \"IKE protocol version.\"\n        },\n        \"authentication_type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"pre-shared-key\",\n            \"certificate\"\
  \n          ],\n          \"description\": \"IKE authentication method.\"\n        }\n      }\n    },\n    \"ipsec_tunnel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"local_address\": {\n          \"type\": \"string\",\n          \"description\": \"Local tunnel IP address assigned by Prisma Access.\"\n        },\n        \"remote_address\": {\n          \"type\": \"string\",\n          \"description\": \"Remote tunnel IP address.\"\n        },\n        \"tunnel_interface\": {\n          \"type\": \"string\",\n          \"description\": \"Tunnel interface name.\"\n        }\n      }\n    },\n    \"tunnel_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\",\n        \"pending\",\n        \"error\"\n      ],\n      \"description\": \"Current IPsec tunnel connection status.\"\n    },\n    \"bandwidth_mbps\": {\n      \"type\": \"integer\",\n      \"description\": \"Allocated bandwidth in Mbps for this remote\
  \ network.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-remote-network-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RemoteNetwork
---
