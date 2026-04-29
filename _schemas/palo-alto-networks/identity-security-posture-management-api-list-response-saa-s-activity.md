---
description: ListResponseSaaSActivity schema from Incident Security Service Posture Management API
layout: schema
name: ListResponseSaaSActivity
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: items
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-list-response-saa-s-activity-schema.json
slug: identity-security-posture-management-api-list-response-saa-s-activity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListResponseSaaSActivity\",\n  \"description\": \"ListResponseSaaSActivity schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-list-response-saa-s-activity-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"format\": \"int64\",\n      \"type\": \"integer\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"userId\": {\n            \"type\": \"string\"\n          },\n          \"tenant\": {\n            \"type\": \"string\"\n          },\n          \"saasInstanceId\": {\n            \"type\": \"string\"\n          },\n          \"appType\"\
  : {\n            \"type\": \"string\"\n          },\n          \"resourceType\": {\n            \"type\": \"string\"\n          },\n          \"resourceName\": {\n            \"type\": \"string\"\n          },\n          \"activityType\": {\n            \"type\": \"string\"\n          },\n          \"clientIP\": {\n            \"type\": \"string\"\n          },\n          \"location\": {\n            \"type\": \"string\"\n          },\n          \"userAgent\": {\n            \"type\": \"string\"\n          },\n          \"summary\": {\n            \"type\": \"string\"\n          },\n          \"rawData\": {\n            \"type\": \"string\"\n          },\n          \"activityDateTime\": {\n            \"format\": \"date-time\",\n            \"type\": \"string\",\n            \"example\": \"2022-03-10T16:15:50+00:00\"\n          },\n          \"createdAt\": {\n            \"format\": \"date-time\",\n            \"type\": \"string\",\n            \"example\": \"2022-03-10T16:15:50+00:00\"\
  \n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-list-response-saa-s-activity-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ListResponseSaaSActivity
---
