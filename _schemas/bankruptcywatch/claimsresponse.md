---
description: Claims register response
layout: schema
name: ClaimsResponse
properties_list:
- description: ''
  name: caseId
  type: string
- description: ''
  name: claims
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/claimsresponse-schema.json
slug: claimsresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/claimsresponse-schema.json\",\n  \"title\": \"ClaimsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Claims register response\",\n  \"properties\": {\n    \"caseId\": {\n      \"type\": \"string\"\n    },\n    \"claims\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Claim\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/claimsresponse-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: ClaimsResponse
---
