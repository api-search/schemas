---
description: A Cortex XSOAR investigation containing war room entries and playbook state.
layout: schema
name: Investigation
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: integer
- description: ''
  name: incidentId
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: modified
  type: string
- description: ''
  name: entries
  type: array
- description: ''
  name: playbookId
  type: string
- description: ''
  name: runningPlaybooks
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-investigation-schema.json
slug: cortex-xsoar-api-investigation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Investigation\",\n  \"description\": \"A Cortex XSOAR investigation containing war room entries and playbook state.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-investigation-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"integer\"\n    },\n    \"incidentId\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"entries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A war room entry in a Cortex\
  \ XSOAR investigation.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"readOnly\": true\n          },\n          \"investigationId\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"integer\",\n            \"description\": \"Entry type: 1 (Note), 2 (Download), 3 (File), 4 (Error), 5 (Pinned), 6 (UserManagement), 7 (Image), 8 (PlaygroundCommand), 9 (PlaybookStatusNote), 10 (Canvas), 11 (Widget), 12 (Summary), 13 (Section), 14 (Table).\"\n          },\n          \"user\": {\n            \"type\": \"string\",\n            \"description\": \"Username of the user who created the entry.\"\n          },\n          \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"modified\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"contents\": {\n            \"type\": \"string\",\n\
  \            \"description\": \"Entry content text.\"\n          },\n          \"humanReadable\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable formatted content.\"\n          },\n          \"tags\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"playbookId\": {\n      \"type\": \"string\"\n    },\n    \"runningPlaybooks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-investigation-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Investigation
---
