---
description: ListResponseSaaSInstanceInfo schema from Incident Security Service Posture Management API
layout: schema
name: ListResponseSaaSInstanceInfo
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: items
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-list-response-saa-s-instance-info-schema.json
slug: identity-security-posture-management-api-list-response-saa-s-instance-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListResponseSaaSInstanceInfo\",\n  \"description\": \"ListResponseSaaSInstanceInfo schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-list-response-saa-s-instance-info-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayName\": {\n            \"type\": \"string\"\n          },\n          \"saasInstanceId\": {\n            \"type\": \"string\"\n          },\n          \"appType\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-list-response-saa-s-instance-info-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ListResponseSaaSInstanceInfo
---
