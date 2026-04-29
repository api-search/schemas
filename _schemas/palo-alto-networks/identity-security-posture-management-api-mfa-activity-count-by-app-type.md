---
description: MfaActivityCountByAppType schema from Incident Security Service Posture Management API
layout: schema
name: MfaActivityCountByAppType
properties_list:
- description: ''
  name: appType
  type: string
- description: ''
  name: count
  type: integer
- description: ''
  name: iconAppType
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-mfa-activity-count-by-app-type-schema.json
slug: identity-security-posture-management-api-mfa-activity-count-by-app-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MfaActivityCountByAppType\",\n  \"description\": \"MfaActivityCountByAppType schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-mfa-activity-count-by-app-type-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appType\": {\n      \"type\": \"string\"\n    },\n    \"count\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"iconAppType\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-mfa-activity-count-by-app-type-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MfaActivityCountByAppType
---
