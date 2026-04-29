---
description: Proof of Claim filing response
layout: schema
name: ProofOfClaimResponse
properties_list:
- description: ''
  name: claimId
  type: string
- description: ''
  name: caseId
  type: string
- description: ''
  name: confirmationNumber
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: filedAt
  type: string
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/proofofclaimresponse-schema.json
slug: proofofclaimresponse
source_filename: proofofclaimresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/proofofclaimresponse-schema.json\",\n  \"title\": \"ProofOfClaimResponse\",\n  \"type\": \"object\",\n  \"description\": \"Proof of Claim filing response\",\n  \"properties\": {\n    \"claimId\": {\n      \"type\": \"string\"\n    },\n    \"caseId\": {\n      \"type\": \"string\"\n    },\n    \"confirmationNumber\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"filedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/proofofclaimresponse-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: ProofOfClaimResponse
---
