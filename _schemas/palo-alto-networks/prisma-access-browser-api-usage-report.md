---
description: UsageReport schema from Palo Alto Networks Prisma Access Browser Management API
layout: schema
name: UsageReport
properties_list:
- description: ''
  name: period
  type: object
- description: Number of unique active users during the period.
  name: active_users
  type: integer
- description: Total browser sessions started during the period.
  name: total_sessions
  type: integer
- description: Total data transferred through the browser in GB.
  name: data_transferred_gb
  type: number
- description: Number of threats blocked by the browser.
  name: threats_blocked
  type: integer
- description: Number of DLP policy events triggered.
  name: dlp_events
  type: integer
- description: Time-series data points for the report.
  name: data_points
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-browser-api-usage-report-schema.json
slug: prisma-access-browser-api-usage-report
source_filename: prisma-access-browser-api-usage-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UsageReport\",\n  \"description\": \"UsageReport schema from Palo Alto Networks Prisma Access Browser Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-usage-report-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"period\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        }\n      }\n    },\n    \"active_users\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unique active users during the period.\"\n    },\n    \"total_sessions\": {\n      \"type\": \"integer\",\n      \"description\": \"Total browser sessions started during the period.\"\n    },\n    \"\
  data_transferred_gb\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"description\": \"Total data transferred through the browser in GB.\"\n    },\n    \"threats_blocked\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of threats blocked by the browser.\"\n    },\n    \"dlp_events\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of DLP policy events triggered.\"\n    },\n    \"data_points\": {\n      \"type\": \"array\",\n      \"description\": \"Time-series data points for the report.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"active_users\": {\n            \"type\": \"integer\"\n          },\n          \"sessions\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-browser-api-usage-report-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: UsageReport
---
