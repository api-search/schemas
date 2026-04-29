---
description: ComplianceStandard schema from Palo Alto Networks Prisma Cloud CSPM API
layout: schema
name: ComplianceStandard
properties_list:
- description: Unique compliance standard identifier.
  name: id
  type: string
- description: Name of the compliance standard.
  name: name
  type: string
- description: Standard description.
  name: description
  type: string
- description: Cloud providers the standard applies to.
  name: cloudType
  type: array
- description: Whether this is a built-in compliance standard.
  name: systemDefault
  type: boolean
- description: Number of policies mapped to this standard.
  name: policiesAssigned
  type: integer
- description: User who created the standard.
  name: createdBy
  type: string
- description: Epoch timestamp of last modification.
  name: lastModifiedTs
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-cspm-api-compliance-standard-schema.json
slug: prisma-cloud-cspm-api-compliance-standard
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComplianceStandard\",\n  \"description\": \"ComplianceStandard schema from Palo Alto Networks Prisma Cloud CSPM API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-compliance-standard-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique compliance standard identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the compliance standard.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Standard description.\"\n    },\n    \"cloudType\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Cloud providers the standard applies to.\"\n    },\n    \"systemDefault\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Whether this is a built-in compliance standard.\"\n    },\n    \"policiesAssigned\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of policies mapped to this standard.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the standard.\"\n    },\n    \"lastModifiedTs\": {\n      \"type\": \"integer\",\n      \"description\": \"Epoch timestamp of last modification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-cspm-api-compliance-standard-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ComplianceStandard
---
