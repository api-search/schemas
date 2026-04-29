---
description: ''
layout: schema
name: Result
properties_list:
- description: Probe server ID
  name: probeid
  type: integer
- description: Test timestamp (Unix)
  name: time
  type: integer
- description: Result status
  name: status
  type: string
- description: Response time in milliseconds
  name: responsetime
  type: integer
- description: Status description
  name: statusdesc
  type: string
- description: Detailed status description
  name: statusdesclong
  type: string
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-pingdom-result-schema.json
slug: solarwinds-pingdom-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Result\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"probeid\": {\n      \"type\": \"integer\",\n      \"description\": \"Probe server ID\"\n    },\n    \"time\": {\n      \"type\": \"integer\",\n      \"description\": \"Test timestamp (Unix)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Result status\"\n    },\n    \"responsetime\": {\n      \"type\": \"integer\",\n      \"description\": \"Response time in milliseconds\"\n    },\n    \"statusdesc\": {\n      \"type\": \"string\",\n      \"description\": \"Status description\"\n    },\n    \"statusdesclong\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed status description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-pingdom-result-schema.json
tags:
- Application Monitoring
- Database Monitoring
- Infrastructure
- IP Address Management
- IT Management
- ITSM
- Log Management
- Network Monitoring
- Observability
title: Result
---
