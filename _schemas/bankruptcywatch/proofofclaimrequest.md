---
description: Proof of Claim filing request
layout: schema
name: ProofOfClaimRequest
properties_list:
- description: ''
  name: creditorName
  type: string
- description: ''
  name: creditorAddress
  type: string
- description: ''
  name: claimAmount
  type: number
- description: ''
  name: securedAmount
  type: number
- description: ''
  name: basisForClaim
  type: string
- description: ''
  name: accountNumber
  type: string
- description: ''
  name: attachmentUrls
  type: array
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/proofofclaimrequest-schema.json
slug: proofofclaimrequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/proofofclaimrequest-schema.json\",\n  \"title\": \"ProofOfClaimRequest\",\n  \"type\": \"object\",\n  \"description\": \"Proof of Claim filing request\",\n  \"required\": [\n    \"creditorName\",\n    \"claimAmount\",\n    \"basisForClaim\"\n  ],\n  \"properties\": {\n    \"creditorName\": {\n      \"type\": \"string\"\n    },\n    \"creditorAddress\": {\n      \"type\": \"string\"\n    },\n    \"claimAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"securedAmount\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"basisForClaim\": {\n      \"type\": \"string\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\"\n    },\n    \"attachmentUrls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/proofofclaimrequest-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: ProofOfClaimRequest
---
