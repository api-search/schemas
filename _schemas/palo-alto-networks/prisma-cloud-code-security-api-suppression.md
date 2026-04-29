---
description: Suppression schema from Palo Alto Networks Prisma Cloud Code Security API
layout: schema
name: Suppression
properties_list:
- description: Unique suppression rule identifier.
  name: suppressionId
  type: string
- description: Checkov policy ID being suppressed.
  name: policyId
  type: string
- description: Human-readable policy name.
  name: policyName
  type: string
- description: Scope of the suppression.
  name: suppressionType
  type: string
- description: Reason provided for the suppression.
  name: justification
  type: string
- description: Email address of the user who created the suppression.
  name: createdBy
  type: string
- description: Timestamp when the suppression was created.
  name: createdAt
  type: string
- description: Expiration date. Null if the suppression does not expire.
  name: expirationDate
  type: string
- description: Number of errors currently suppressed by this rule.
  name: suppressedErrorCount
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-code-security-api-suppression-schema.json
slug: prisma-cloud-code-security-api-suppression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Suppression\",\n  \"description\": \"Suppression schema from Palo Alto Networks Prisma Cloud Code Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-suppression-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"suppressionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique suppression rule identifier.\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Checkov policy ID being suppressed.\"\n    },\n    \"policyName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable policy name.\"\n    },\n    \"suppressionType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Policy\",\n        \"Resources\",\n        \"Accounts\",\n        \"Tags\"\n      ],\n      \"description\": \"Scope of the\
  \ suppression.\"\n    },\n    \"justification\": {\n      \"type\": \"string\",\n      \"description\": \"Reason provided for the suppression.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the user who created the suppression.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the suppression was created.\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Expiration date. Null if the suppression does not expire.\"\n    },\n    \"suppressedErrorCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of errors currently suppressed by this rule.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-code-security-api-suppression-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Suppression
---
