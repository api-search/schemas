---
description: PersonalData schema from Adyen API
layout: schema
name: PersonalData
properties_list:
- description: The date of birth of the person. The date should be in ISO-8601 format yyyy-mm-dd (e.g. 2000-01-31).
  name: dateOfBirth
  type: string
- description: An ID number of the person.
  name: idNumber
  type: string
- description: The nationality of the person represented by a two-character country code. >The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL').
  name: nationality
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-personal-data-schema.json
slug: configuration-webhooks-personal-data
source_filename: configuration-webhooks-personal-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-personal-data-schema.json\",\n  \"title\": \"PersonalData\",\n  \"description\": \"PersonalData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dateOfBirth\": {\n      \"description\": \"The date of birth of the person.\\nThe date should be in ISO-8601 format yyyy-mm-dd (e.g. 2000-01-31).\",\n      \"type\": \"string\"\n    },\n    \"idNumber\": {\n      \"description\": \"An ID number of the person.\",\n      \"type\": \"string\"\n    },\n    \"nationality\": {\n      \"description\": \"The nationality of the person represented by a two-character country code.\\n>The permitted country codes are defined in ISO-3166-1 alpha-2 (e.g. 'NL').\",\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-personal-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PersonalData
---
