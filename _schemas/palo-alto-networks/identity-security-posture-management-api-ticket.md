---
description: Ticket schema from Incident Security Service Posture Management API
layout: schema
name: Ticket
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: tenant
  type: string
- description: ''
  name: saasInstanceId
  type: string
- description: ''
  name: resourceIds
  type: string
- description: ''
  name: feature
  type: string
- description: ''
  name: users
  type: string
- description: ''
  name: integrationId
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: ticketKey
  type: string
- description: ''
  name: ticketUrl
  type: string
- description: ''
  name: summary
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-ticket-schema.json
slug: identity-security-posture-management-api-ticket
source_filename: identity-security-posture-management-api-ticket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Ticket\",\n  \"description\": \"Ticket schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-ticket-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"tenant\": {\n      \"type\": \"string\"\n    },\n    \"saasInstanceId\": {\n      \"type\": \"string\"\n    },\n    \"resourceIds\": {\n      \"type\": \"string\"\n    },\n    \"feature\": {\n      \"type\": \"string\"\n    },\n    \"users\": {\n      \"type\": \"string\"\n    },\n    \"integrationId\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"ticketKey\": {\n      \"type\": \"string\"\n    },\n    \"ticketUrl\": {\n      \"type\": \"string\"\n    },\n    \"summary\"\
  : {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"example\": \"2022-03-10T16:15:50+00:00\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-ticket-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Ticket
---
