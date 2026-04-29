---
description: IKEGateway schema from Palo Alto Networks SASE Configuration Orchestration API
layout: schema
name: IKEGateway
properties_list:
- description: Public IP address of the remote peer gateway.
  name: peer_ip
  type: string
- description: IKE peer identity.
  name: peer_id
  type: string
- description: Prisma Access local IKE gateway IP address.
  name: local_ip
  type: string
- description: IKE protocol version.
  name: ike_version
  type: string
- description: IKE authentication method.
  name: authentication_type
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-config-orchestration-api-ike-gateway-schema.json
slug: sase-config-orchestration-api-ike-gateway
source_filename: sase-config-orchestration-api-ike-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IKEGateway\",\n  \"description\": \"IKEGateway schema from Palo Alto Networks SASE Configuration Orchestration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-ike-gateway-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"peer_ip\": {\n      \"type\": \"string\",\n      \"description\": \"Public IP address of the remote peer gateway.\"\n    },\n    \"peer_id\": {\n      \"type\": \"string\",\n      \"description\": \"IKE peer identity.\"\n    },\n    \"local_ip\": {\n      \"type\": \"string\",\n      \"description\": \"Prisma Access local IKE gateway IP address.\"\n    },\n    \"ike_version\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IKEv1\",\n        \"IKEv2\"\n      ],\n      \"description\": \"IKE protocol version.\"\n    },\n    \"authentication_type\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pre-shared-key\",\n        \"certificate\"\n      ],\n      \"description\": \"IKE authentication method.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-ike-gateway-schema.json
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
