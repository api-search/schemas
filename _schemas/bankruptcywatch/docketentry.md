---
description: A single docket entry in a bankruptcy case
layout: schema
name: DocketEntry
properties_list:
- description: ''
  name: entryId
  type: string
- description: ''
  name: caseId
  type: string
- description: ''
  name: entryNumber
  type: integer
- description: ''
  name: dateFiled
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: documentUrl
  type: string
- description: ''
  name: filer
  type: string
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/docketentry-schema.json
slug: docketentry
source_filename: docketentry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bankruptcywatch/json-schema/docketentry-schema.json\",\n  \"title\": \"DocketEntry\",\n  \"type\": \"object\",\n  \"description\": \"A single docket entry in a bankruptcy case\",\n  \"properties\": {\n    \"entryId\": {\n      \"type\": \"string\"\n    },\n    \"caseId\": {\n      \"type\": \"string\"\n    },\n    \"entryNumber\": {\n      \"type\": \"integer\"\n    },\n    \"dateFiled\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"documentUrl\": {\n      \"type\": \"string\"\n    },\n    \"filer\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bankruptcywatch/refs/heads/main/json-schema/docketentry-schema.json
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: DocketEntry
---
