---
description: IKEGateway schema from Palo Alto Networks Prisma Access Configuration API
layout: schema
name: IKEGateway
properties_list:
- description: Unique identifier for the IKE gateway.
  name: id
  type: string
- description: Name of the IKE gateway.
  name: name
  type: string
- description: IKE protocol version.
  name: version
  type: string
- description: Peer IP address configuration.
  name: peer_address
  type: object
- description: IKE authentication configuration.
  name: authentication
  type: object
- description: ''
  name: local_id
  type: object
- description: ''
  name: peer_id
  type: object
- description: ''
  name: folder
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-api-ike-gateway-schema.json
slug: prisma-access-api-ike-gateway
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IKEGateway\",\n  \"description\": \"IKEGateway schema from Palo Alto Networks Prisma Access Configuration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-ike-gateway-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the IKE gateway.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the IKE gateway.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ikev1\",\n        \"ikev2\",\n        \"ikev2-preferred\"\n      ],\n      \"default\": \"ikev2-preferred\",\n      \"description\": \"IKE protocol version.\"\n    },\n    \"peer_address\": {\n      \"type\": \"object\",\n      \"description\": \"Peer IP address\
  \ configuration.\",\n      \"properties\": {\n        \"ip\": {\n          \"type\": \"string\",\n          \"format\": \"ipv4\",\n          \"description\": \"Static peer IP address.\"\n        },\n        \"dynamic\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the peer address is dynamic.\"\n        }\n      }\n    },\n    \"authentication\": {\n      \"type\": \"object\",\n      \"description\": \"IKE authentication configuration.\",\n      \"properties\": {\n        \"pre_shared_key\": {\n          \"type\": \"string\",\n          \"description\": \"Pre-shared key for IKE authentication.\"\n        },\n        \"certificate\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"local_certificate\": {\n              \"type\": \"string\",\n              \"description\": \"Local certificate profile name.\"\n            }\n          }\n        }\n      }\n    },\n    \"local_id\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ipaddr\",\n            \"keyid\",\n            \"fqdn\",\n            \"ufqdn\"\n          ]\n        },\n        \"id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"peer_id\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ipaddr\",\n            \"keyid\",\n            \"fqdn\",\n            \"ufqdn\"\n          ]\n        },\n        \"id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"peer_address\",\n    \"authentication\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-api-ike-gateway-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IKEGateway
---
