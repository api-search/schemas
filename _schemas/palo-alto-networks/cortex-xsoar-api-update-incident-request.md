---
description: UpdateIncidentRequest schema from Palo Alto Networks Cortex XSOAR REST API
layout: schema
name: UpdateIncidentRequest
properties_list:
- description: ID of the incident to update.
  name: id
  type: string
- description: Incident version for optimistic locking. Retrieve from a prior GET request.
  name: version
  type: integer
- description: ''
  name: status
  type: integer
- description: ''
  name: severity
  type: integer
- description: ''
  name: owner
  type: string
- description: ''
  name: details
  type: string
- description: ''
  name: closeReason
  type: string
- description: ''
  name: closeNotes
  type: string
- description: ''
  name: CustomFields
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-update-incident-request-schema.json
slug: cortex-xsoar-api-update-incident-request
source_filename: cortex-xsoar-api-update-incident-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateIncidentRequest\",\n  \"description\": \"UpdateIncidentRequest schema from Palo Alto Networks Cortex XSOAR REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-update-incident-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the incident to update.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Incident version for optimistic locking. Retrieve from a prior GET request.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"enum\": [\n        0,\n        1,\n        2,\n        3\n      ]\n    },\n    \"severity\": {\n      \"type\": \"integer\",\n      \"enum\": [\n        0,\n        1,\n        2,\n        3,\n        4,\n        5\n      ]\n    },\n   \
  \ \"owner\": {\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"type\": \"string\"\n    },\n    \"closeReason\": {\n      \"type\": \"string\"\n    },\n    \"closeNotes\": {\n      \"type\": \"string\"\n    },\n    \"CustomFields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-update-incident-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: UpdateIncidentRequest
---
