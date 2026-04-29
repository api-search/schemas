---
description: ListResponseMfaActivity schema from Incident Security Service Posture Management API
layout: schema
name: ListResponseMfaActivity
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: items
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-list-response-mfa-activity-schema.json
slug: identity-security-posture-management-api-list-response-mfa-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListResponseMfaActivity\",\n  \"description\": \"ListResponseMfaActivity schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-list-response-mfa-activity-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"tenant\": {\n            \"type\": \"string\"\n          },\n          \"userId\": {\n            \"type\": \"string\"\n          },\n          \"idpId\": {\n            \"type\": \"string\"\n          },\n          \"idpType\": {\n    \
  \        \"type\": \"string\"\n          },\n          \"mfaStrength\": {\n            \"type\": \"string\"\n          },\n          \"admin\": {\n            \"type\": \"boolean\"\n          },\n          \"appType\": {\n            \"type\": \"string\"\n          },\n          \"appId\": {\n            \"type\": \"string\"\n          },\n          \"timestamp\": {\n            \"format\": \"date-time\",\n            \"type\": \"string\",\n            \"example\": \"2022-03-10T16:15:50+00:00\"\n          },\n          \"mfaFactors\": {\n            \"type\": \"string\"\n          },\n          \"saasProviderMfaType\": {\n            \"type\": \"string\"\n          },\n          \"fullName\": {\n            \"type\": \"string\"\n          },\n          \"email\": {\n            \"type\": \"string\"\n          },\n          \"ipAddress\": {\n            \"type\": \"string\"\n          },\n          \"location\": {\n            \"type\": \"string\"\n          },\n          \"ticketKey\"\
  : {\n            \"type\": \"string\"\n          },\n          \"ticketUrl\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-list-response-mfa-activity-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ListResponseMfaActivity
---
