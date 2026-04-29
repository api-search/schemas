---
description: PolicyInput schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: PolicyInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: policyType
  type: string
- description: ''
  name: severity
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: recommendation
  type: string
- description: ''
  name: cloudType
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: rule
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-policy-input-schema.json
slug: prisma-cloud-cspm-api-policy-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyInput\",\n  \"description\": \"PolicyInput schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-policy-input-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"policyType\": {\n      \"type\": \"string\"\n    },\n    \"severity\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"recommendation\": {\n      \"type\": \"string\"\n    },\n    \"cloudType\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"rule\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"name\",\n        \"criteria\",\n        \"type\"\n      ],\n      \"properties\"\
  : {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"criteria\": {\n          \"type\": \"string\",\n          \"description\": \"RQL query for the policy rule.\"\n        },\n        \"type\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"policyType\",\n    \"severity\",\n    \"rule\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-policy-input-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PolicyInput
---
