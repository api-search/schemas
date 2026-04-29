---
description: CreateIncidentRequest schema from Palo Alto Networks Cortex XSOAR REST API
layout: schema
name: CreateIncidentRequest
properties_list:
- description: Incident name.
  name: name
  type: string
- description: Incident type name.
  name: type
  type: string
- description: ''
  name: severity
  type: integer
- description: ''
  name: owner
  type: string
- description: ''
  name: occurred
  type: string
- description: ''
  name: details
  type: string
- description: ''
  name: labels
  type: array
- description: Whether to automatically create an investigation for this incident.
  name: createInvestigation
  type: boolean
- description: ''
  name: CustomFields
  type: object
- description: ''
  name: rawJson
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-create-incident-request-schema.json
slug: cortex-xsoar-api-create-incident-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateIncidentRequest\",\n  \"description\": \"CreateIncidentRequest schema from Palo Alto Networks Cortex XSOAR REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-create-incident-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Incident name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Incident type name.\"\n    },\n    \"severity\": {\n      \"type\": \"integer\",\n      \"enum\": [\n        0,\n        1,\n        2,\n        3,\n        4,\n        5\n      ]\n    },\n    \"owner\": {\n      \"type\": \"string\"\n    },\n    \"occurred\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"details\": {\n      \"type\": \"string\"\n    },\n    \"labels\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"createInvestigation\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether to automatically create an investigation for this incident.\"\n    },\n    \"CustomFields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    },\n    \"rawJson\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-create-incident-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CreateIncidentRequest
---
