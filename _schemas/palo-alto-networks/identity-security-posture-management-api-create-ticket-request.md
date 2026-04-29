---
description: CreateTicketRequest schema from Incident Security Service Posture Management API
layout: schema
name: CreateTicketRequest
properties_list:
- description: ''
  name: resourceIds
  type: array
- description: ''
  name: feature
  type: string
- description: ''
  name: integrationId
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: issueTypeId
  type: string
- description: ''
  name: summary
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: settings
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-create-ticket-request-schema.json
slug: identity-security-posture-management-api-create-ticket-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTicketRequest\",\n  \"description\": \"CreateTicketRequest schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-create-ticket-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"feature\": {\n      \"enum\": [\n        \"ENROLLMENT\",\n        \"ACTIVITY\",\n        \"LOGOUT\",\n        \"IDENTITY_NHI\",\n        \"IDENTITY_ACTIVITY\"\n      ],\n      \"type\": \"string\"\n    },\n    \"integrationId\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"issueTypeId\": {\n      \"type\": \"string\"\n    },\n    \"summary\": {\n      \"type\"\
  : \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"resourceIds\",\n    \"feature\",\n    \"integrationId\",\n    \"type\",\n    \"issueTypeId\",\n    \"summary\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-create-ticket-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CreateTicketRequest
---
