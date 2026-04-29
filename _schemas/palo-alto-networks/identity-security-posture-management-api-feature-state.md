---
description: FeatureState schema from Incident Security Service Posture Management API
layout: schema
name: FeatureState
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: lastScannedAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-feature-state-schema.json
slug: identity-security-posture-management-api-feature-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FeatureState\",\n  \"description\": \"FeatureState schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-feature-state-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"lastScannedAt\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"example\": \"2022-03-10T16:15:50+00:00\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-feature-state-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: FeatureState
---
