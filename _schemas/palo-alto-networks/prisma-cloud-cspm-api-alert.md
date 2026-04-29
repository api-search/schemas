---
description: Alert schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: Alert
properties_list:
- description: Unique alert identifier.
  name: id
  type: string
- description: Current alert status.
  name: status
  type: string
- description: Reason for the current alert status.
  name: reason
  type: string
- description: Epoch timestamp in milliseconds when the alert was first generated.
  name: firstSeen
  type: integer
- description: Epoch timestamp in milliseconds when the alert was last seen.
  name: lastSeen
  type: integer
- description: Epoch timestamp in milliseconds of the alert.
  name: alertTime
  type: integer
- description: Policy that generated this alert.
  name: policy
  type: object
- description: Cloud resource associated with the alert.
  name: resource
  type: object
- description: ''
  name: riskDetail
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-alert-schema.json
slug: prisma-cloud-cspm-api-alert
source_filename: prisma-cloud-cspm-api-alert-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Alert\",\n  \"description\": \"Alert schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-alert-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique alert identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"open\",\n        \"dismissed\",\n        \"snoozed\",\n        \"resolved\"\n      ],\n      \"description\": \"Current alert status.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the current alert status.\"\n    },\n    \"firstSeen\": {\n      \"type\": \"integer\",\n      \"description\": \"Epoch timestamp in milliseconds when the alert was first generated.\"\n    },\n    \"\
  lastSeen\": {\n      \"type\": \"integer\",\n      \"description\": \"Epoch timestamp in milliseconds when the alert was last seen.\"\n    },\n    \"alertTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Epoch timestamp in milliseconds of the alert.\"\n    },\n    \"policy\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"policyId\": {\n          \"type\": \"string\"\n        },\n        \"policyType\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"severity\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"critical\",\n            \"high\",\n            \"medium\",\n            \"low\",\n            \"informational\"\n          ]\n        },\n        \"recommendation\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Policy that generated this alert.\"\n    },\n    \"resource\": {\n      \"type\": \"object\",\n      \"\
  properties\": {\n        \"rrn\": {\n          \"type\": \"string\",\n          \"description\": \"Prisma Cloud Resource RRN.\"\n        },\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"cloudType\": {\n          \"type\": \"string\"\n        },\n        \"accountId\": {\n          \"type\": \"string\"\n        },\n        \"accountName\": {\n          \"type\": \"string\"\n        },\n        \"regionId\": {\n          \"type\": \"string\"\n        },\n        \"resourceType\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Cloud resource associated with the alert.\"\n    },\n    \"riskDetail\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"score\": {\n          \"type\": \"integer\"\n        },\n        \"rating\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-alert-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Alert
---
