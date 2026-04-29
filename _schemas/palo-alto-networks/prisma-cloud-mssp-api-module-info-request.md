---
description: 'ModuleInfoRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)'
layout: schema
name: ModuleInfoRequest
properties_list:
- description: ''
  name: featureName
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: additionalData
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-mssp-api-module-info-request-schema.json
slug: prisma-cloud-mssp-api-module-info-request
source_filename: prisma-cloud-mssp-api-module-info-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModuleInfoRequest\",\n  \"description\": \"ModuleInfoRequest schema from Prisma Cloud: Managed Security Service Provider (MSSP)\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-module-info-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"featureName\": {\n      \"pattern\": \"iam-security\",\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"additionalData\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\": [\n    \"enabled\",\n    \"featureName\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-mssp-api-module-info-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ModuleInfoRequest
---
