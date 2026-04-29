---
description: Localization schema from Adyen API
layout: schema
name: Localization
properties_list:
- description: Language of the terminal.
  name: language
  type: string
- description: Secondary language of the terminal.
  name: secondaryLanguage
  type: string
- description: The time zone of the terminal.
  name: timezone
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-localization-schema.json
slug: management-localization
source_filename: management-localization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-localization-schema.json\",\n  \"title\": \"Localization\",\n  \"description\": \"Localization schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"language\": {\n      \"description\": \"Language of the terminal.\",\n      \"type\": \"string\"\n    },\n    \"secondaryLanguage\": {\n      \"description\": \"Secondary language of the terminal.\",\n      \"type\": \"string\"\n    },\n    \"timezone\": {\n      \"description\": \"The time zone of the terminal.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-localization-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Localization
---
