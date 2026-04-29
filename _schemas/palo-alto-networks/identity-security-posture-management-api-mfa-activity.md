---
description: MfaActivity schema from Incident Security Service Posture Management API
layout: schema
name: MfaActivity
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: tenant
  type: string
- description: ''
  name: userId
  type: string
- description: ''
  name: idpId
  type: string
- description: ''
  name: idpType
  type: string
- description: ''
  name: mfaStrength
  type: string
- description: ''
  name: admin
  type: boolean
- description: ''
  name: appType
  type: string
- description: ''
  name: appId
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: mfaFactors
  type: string
- description: ''
  name: saasProviderMfaType
  type: string
- description: ''
  name: fullName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: ipAddress
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: ticketKey
  type: string
- description: ''
  name: ticketUrl
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-mfa-activity-schema.json
slug: identity-security-posture-management-api-mfa-activity
source_filename: identity-security-posture-management-api-mfa-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MfaActivity\",\n  \"description\": \"MfaActivity schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-mfa-activity-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"tenant\": {\n      \"type\": \"string\"\n    },\n    \"userId\": {\n      \"type\": \"string\"\n    },\n    \"idpId\": {\n      \"type\": \"string\"\n    },\n    \"idpType\": {\n      \"type\": \"string\"\n    },\n    \"mfaStrength\": {\n      \"type\": \"string\"\n    },\n    \"admin\": {\n      \"type\": \"boolean\"\n    },\n    \"appType\": {\n      \"type\": \"string\"\n    },\n    \"appId\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"format\": \"date-time\",\n      \"type\"\
  : \"string\",\n      \"example\": \"2022-03-10T16:15:50+00:00\"\n    },\n    \"mfaFactors\": {\n      \"type\": \"string\"\n    },\n    \"saasProviderMfaType\": {\n      \"type\": \"string\"\n    },\n    \"fullName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"ticketKey\": {\n      \"type\": \"string\"\n    },\n    \"ticketUrl\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-mfa-activity-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MfaActivity
---
