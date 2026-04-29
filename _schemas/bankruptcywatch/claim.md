---
description: A claim in a bankruptcy case claims register
layout: schema
name: Claim
properties_list:
- description: ''
  name: claimId
  type: string
- description: ''
  name: caseId
  type: string
- description: ''
  name: claimNumber
  type: string
- description: ''
  name: creditorName
  type: string
- description: ''
  name: claimAmount
  type: number
- description: ''
  name: securedAmount
  type: number
- description: ''
  name: unsecuredAmount
  type: number
- description: ''
  name: status
  type: string
- description: ''
  name: dateFiled
  type: string
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/claim-schema.json
slug: claim
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/claim-schema.json\",\n  \"title\": \"Claim\",\n  \"type\": \"object\",\n  \"description\": \"A claim in a bankruptcy case claims register\",\n  \"properties\": {\n    \"claimId\": {\n      \"type\": \"string\"\n    },\n    \"caseId\": {\n      \"type\": \"string\"\n    },\n    \"claimNumber\": {\n      \"type\": \"string\"\n    },\n    \"creditorName\": {\n      \"type\": \"string\"\n    },\n    \"claimAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"securedAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"unsecuredAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"dateFiled\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/claim-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: Claim
---
