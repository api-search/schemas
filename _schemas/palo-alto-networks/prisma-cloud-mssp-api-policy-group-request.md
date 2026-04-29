---
description: 'PolicyGroupRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: PolicyGroupRequest
properties_list:
- description: Name of the policy group.
  name: name
  type: string
- description: Policies assigned to this policy group.
  name: policies
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-policy-group-request-schema.json
slug: prisma-cloud-mssp-api-policy-group-request
source_filename: prisma-cloud-mssp-api-policy-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PolicyGroupRequest\",\n  \"description\": \"PolicyGroupRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-policy-group-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"maxLength\": 63,\n      \"minLength\": 3,\n      \"type\": \"string\",\n      \"description\": \"Name of the policy group.\"\n    },\n    \"policies\": {\n      \"type\": \"array\",\n      \"description\": \"Policies assigned to this policy group.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Policies assigned to this policy group.\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-policy-group-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PolicyGroupRequest
---
