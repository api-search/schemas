---
description: Bankruptcy case search results
layout: schema
name: CaseSearchResponse
properties_list:
- description: ''
  name: cases
  type: array
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: pageSize
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/casesearchresponse-schema.json
slug: casesearchresponse
source_filename: casesearchresponse-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/casesearchresponse-schema.json\",\n  \"title\": \"CaseSearchResponse\",\n  \"type\": \"object\",\n  \"description\": \"Bankruptcy case search results\",\n  \"properties\": {\n    \"cases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Case\"\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"pageSize\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/casesearchresponse-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: CaseSearchResponse
---
