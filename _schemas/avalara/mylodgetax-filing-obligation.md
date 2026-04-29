---
description: FilingObligation schema from Avalara API
layout: schema
name: FilingObligation
properties_list:
- description: ''
  name: jurisdiction
  type: string
- description: ''
  name: taxType
  type: string
- description: ''
  name: filingFrequency
  type: string
- description: ''
  name: nextDueDate
  type: string
- description: ''
  name: registrationRequired
  type: boolean
- description: ''
  name: registrationUrl
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/mylodgetax-filing-obligation-schema.json
slug: mylodgetax-filing-obligation
source_filename: mylodgetax-filing-obligation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/mylodgetax-filing-obligation-schema.json\",\n  \"title\": \"FilingObligation\",\n  \"description\": \"FilingObligation schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jurisdiction\": {\n      \"type\": \"string\"\n    },\n    \"taxType\": {\n      \"type\": \"string\"\n    },\n    \"filingFrequency\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Monthly\",\n        \"Quarterly\",\n        \"Annual\"\n      ]\n    },\n    \"nextDueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"registrationRequired\": {\n      \"type\": \"boolean\"\n    },\n    \"registrationUrl\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/mylodgetax-filing-obligation-schema.json
tags:
- Taxes
title: FilingObligation
---
