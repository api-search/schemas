---
description: UnlinkTicketRequest schema from Incident Security Service Posture Management API
layout: schema
name: UnlinkTicketRequest
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: resourceIds
  type: array
- description: ''
  name: feature
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-unlink-ticket-request-schema.json
slug: identity-security-posture-management-api-unlink-ticket-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UnlinkTicketRequest\",\n  \"description\": \"UnlinkTicketRequest schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-unlink-ticket-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"resourceIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"feature\": {\n      \"enum\": [\n        \"ENROLLMENT\",\n        \"ACTIVITY\",\n        \"LOGOUT\",\n        \"IDENTITY_NHI\",\n        \"IDENTITY_ACTIVITY\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"feature\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-unlink-ticket-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: UnlinkTicketRequest
---
