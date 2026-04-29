---
description: Docket entries response
layout: schema
name: DocketResponse
properties_list:
- description: ''
  name: caseId
  type: string
- description: ''
  name: entries
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/docketresponse-schema.json
slug: docketresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/docketresponse-schema.json\",\n  \"title\": \"DocketResponse\",\n  \"type\": \"object\",\n  \"description\": \"Docket entries response\",\n  \"properties\": {\n    \"caseId\": {\n      \"type\": \"string\"\n    },\n    \"entries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DocketEntry\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/docketresponse-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: DocketResponse
---
