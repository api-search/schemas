---
description: RemoteNetworkRequest schema from Palo Alto Networks SASE Configuration Orchestration API
layout: schema
name: RemoteNetworkRequest
properties_list:
- description: Display name for the remote network.
  name: name
  type: string
- description: Optional description.
  name: description
  type: string
- description: Prisma Access gateway location name.
  name: location
  type: string
- description: Network subnets at the remote site in CIDR notation.
  name: subnets
  type: array
- description: ''
  name: ike_gateway
  type: object
- description: Requested bandwidth allocation in Mbps.
  name: bandwidth_mbps
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-config-orchestration-api-remote-network-request-schema.json
slug: sase-config-orchestration-api-remote-network-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RemoteNetworkRequest\",\n  \"description\": \"RemoteNetworkRequest schema from Palo Alto Networks SASE Configuration Orchestration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-remote-network-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the remote network.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Prisma Access gateway location name.\"\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Network subnets at the remote site in CIDR notation.\"\n\
  \    },\n    \"ike_gateway\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"peer_ip\"\n      ],\n      \"properties\": {\n        \"peer_ip\": {\n          \"type\": \"string\",\n          \"description\": \"Public IP address of the remote peer gateway.\"\n        },\n        \"peer_id\": {\n          \"type\": \"string\",\n          \"description\": \"IKE peer identity. Defaults to the peer IP if omitted.\"\n        },\n        \"ike_version\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"IKEv1\",\n            \"IKEv2\"\n          ],\n          \"default\": \"IKEv2\"\n        },\n        \"authentication_type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"pre-shared-key\",\n            \"certificate\"\n          ],\n          \"default\": \"pre-shared-key\"\n        },\n        \"pre_shared_key\": {\n          \"type\": \"string\",\n          \"description\": \"Pre-shared key for IKE authentication.\",\n     \
  \     \"writeOnly\": true\n        }\n      }\n    },\n    \"bandwidth_mbps\": {\n      \"type\": \"integer\",\n      \"description\": \"Requested bandwidth allocation in Mbps.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"location\",\n    \"subnets\",\n    \"ike_gateway\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-remote-network-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: RemoteNetworkRequest
---
