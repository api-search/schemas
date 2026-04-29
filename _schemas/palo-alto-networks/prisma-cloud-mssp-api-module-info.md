---
description: 'ModuleInfo schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: ModuleInfo
properties_list:
- description: ''
  name: feature_name
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: billing_type
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: additional_data
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-module-info-schema.json
slug: prisma-cloud-mssp-api-module-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModuleInfo\",\n  \"description\": \"ModuleInfo schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-module-info-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"feature_name\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"billing_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TRIAL\",\n        \"BUY\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PROVISION_STARTED\",\n        \"PROVISION_SUCCESSFUL\",\n        \"PROVISION_FAILED\"\n      ]\n    },\n    \"additional_data\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\"\
  : [\n    \"feature_name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-module-info-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ModuleInfo
---
