---
description: IPSecTunnel schema from Palo Alto Networks Prisma Access Configuration API
layout: schema
name: IPSecTunnel
properties_list:
- description: Unique identifier for the IPSec tunnel.
  name: id
  type: string
- description: Name of the IPSec tunnel.
  name: name
  type: string
- description: Auto-key IKE configuration for the tunnel.
  name: auto_key
  type: object
- description: ''
  name: tunnel_monitor
  type: object
- description: Whether anti-replay protection is enabled.
  name: anti_replay
  type: boolean
- description: ''
  name: folder
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-api-ip-sec-tunnel-schema.json
slug: prisma-access-api-ip-sec-tunnel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IPSecTunnel\",\n  \"description\": \"IPSecTunnel schema from Palo Alto Networks Prisma Access Configuration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-ip-sec-tunnel-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the IPSec tunnel.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the IPSec tunnel.\"\n    },\n    \"auto_key\": {\n      \"type\": \"object\",\n      \"description\": \"Auto-key IKE configuration for the tunnel.\",\n      \"properties\": {\n        \"ike_gateway\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n     \
  \           \"type\": \"string\",\n                \"description\": \"Name of the IKE gateway to use.\"\n              }\n            }\n          }\n        },\n        \"ipsec_crypto_profile\": {\n          \"type\": \"string\",\n          \"description\": \"IPSec crypto profile name.\"\n        }\n      }\n    },\n    \"tunnel_monitor\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"enable\": {\n          \"type\": \"boolean\"\n        },\n        \"destination_ip\": {\n          \"type\": \"string\",\n          \"format\": \"ipv4\"\n        },\n        \"proxy_id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"anti_replay\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether anti-replay protection is enabled.\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"auto_key\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-ip-sec-tunnel-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IPSecTunnel
---
