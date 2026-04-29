---
description: IKEGatewayConfig schema from Palo Alto Networks SASE Configuration Orchestration API
layout: schema
name: IKEGatewayConfig
properties_list:
- description: Public IP address of the remote peer gateway.
  name: peer_ip
  type: string
- description: IKE peer identity. Defaults to the peer IP if omitted.
  name: peer_id
  type: string
- description: ''
  name: ike_version
  type: string
- description: ''
  name: authentication_type
  type: string
- description: Pre-shared key for IKE authentication.
  name: pre_shared_key
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-config-orchestration-api-ike-gateway-config-schema.json
slug: sase-config-orchestration-api-ike-gateway-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IKEGatewayConfig\",\n  \"description\": \"IKEGatewayConfig schema from Palo Alto Networks SASE Configuration Orchestration API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-ike-gateway-config-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"peer_ip\": {\n      \"type\": \"string\",\n      \"description\": \"Public IP address of the remote peer gateway.\"\n    },\n    \"peer_id\": {\n      \"type\": \"string\",\n      \"description\": \"IKE peer identity. Defaults to the peer IP if omitted.\"\n    },\n    \"ike_version\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IKEv1\",\n        \"IKEv2\"\n      ],\n      \"default\": \"IKEv2\"\n    },\n    \"authentication_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pre-shared-key\",\n        \"certificate\"\
  \n      ],\n      \"default\": \"pre-shared-key\"\n    },\n    \"pre_shared_key\": {\n      \"type\": \"string\",\n      \"description\": \"Pre-shared key for IKE authentication.\",\n      \"writeOnly\": true\n    }\n  },\n  \"required\": [\n    \"peer_ip\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-config-orchestration-api-ike-gateway-config-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IKEGatewayConfig
---
