---
description: API usage statistics for the authenticated API key.
layout: schema
name: ApiStats
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: data
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/threat-vault-api-api-stats-schema.json
slug: threat-vault-api-api-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApiStats\",\n  \"description\": \"API usage statistics for the authenticated API key.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-api-stats-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"api_key\": {\n          \"type\": \"string\",\n          \"description\": \"Redacted API key identifier.\"\n        },\n        \"quota\": {\n          \"type\": \"integer\",\n          \"description\": \"Daily request quota.\"\n        },\n        \"remaining\": {\n          \"type\": \"integer\",\n          \"description\": \"Remaining requests in the current day.\"\n        },\n        \"used\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of\
  \ requests used today.\"\n        },\n        \"reset_time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the quota resets.\"\n        },\n        \"endpoint_usage\": {\n          \"type\": \"object\",\n          \"description\": \"Request counts broken down by endpoint.\",\n          \"additionalProperties\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/threat-vault-api-api-stats-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ApiStats
---
