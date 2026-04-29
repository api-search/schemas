---
description: PhoneNumber schema from Adyen API
layout: schema
name: PhoneNumber
properties_list:
- description: The full phone number, including the country code. For example, **+3112345678**.
  name: number
  type: string
- description: 'The type of phone number. Possible values: **mobile**, **landline**, **sip**, **fax.**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-phone-number-schema.json
slug: legal-entity-phone-number
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-phone-number-schema.json\",\n  \"title\": \"PhoneNumber\",\n  \"description\": \"PhoneNumber schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"description\": \"The full phone number, including the country code. For example, **+3112345678**.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of phone number.\\n Possible values: **mobile**, **landline**, **sip**, **fax.** \",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"number\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-phone-number-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PhoneNumber
---
