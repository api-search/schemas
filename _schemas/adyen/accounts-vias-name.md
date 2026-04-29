---
description: ViasName schema from Adyen API
layout: schema
name: ViasName
properties_list:
- description: The first name.
  name: firstName
  type: string
- description: 'The gender. >The following values are permitted: `MALE`, `FEMALE`, `UNKNOWN`.'
  name: gender
  type: string
- description: The name's infix, if applicable. >A maximum length of twenty (20) characters is imposed.
  name: infix
  type: string
- description: The last name.
  name: lastName
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-vias-name-schema.json
slug: accounts-vias-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-vias-name-schema.json\",\n  \"title\": \"ViasName\",\n  \"description\": \"ViasName schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"description\": \"The first name.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"gender\": {\n      \"description\": \"The gender.\\n>The following values are permitted: `MALE`, `FEMALE`, `UNKNOWN`.\",\n      \"enum\": [\n        \"MALE\",\n        \"FEMALE\",\n        \"UNKNOWN\"\n      ],\n      \"maxLength\": 1,\n      \"type\": \"string\"\n    },\n    \"infix\": {\n      \"description\": \"The name's infix, if applicable.\\n>A maximum length of twenty (20) characters is imposed.\",\n      \"maxLength\": 20,\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"The\
  \ last name.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-vias-name-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ViasName
---
