---
description: ''
layout: schema
name: SecFiling
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: filingDate
  type: string
- description: ''
  name: periodOfReport
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: secUrl
  type: string
- description: ''
  name: documentUrl
  type: string
provider_name: Archrock
provider_slug: archrock
schema_file: json-schema/archrock-investor-relations-api-sec-filing-schema.json
slug: archrock-investor-relations-api-sec-filing
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-sec-filing-schema.json\",\n  \"title\": \"SecFiling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"10-K\",\n        \"10-Q\",\n        \"8-K\",\n        \"DEF14A\",\n        \"SC13G\"\n      ]\n    },\n    \"filingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"periodOfReport\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"secUrl\": {\n      \"type\": \"string\"\n    },\n    \"documentUrl\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-sec-filing-schema.json
tags:
- Natural Gas
- Compression Services
- Oil And Gas
- Energy
- Industrial
- 'NYSE: AROC'
title: SecFiling
---
