---
description: BirthData schema from Adyen API
layout: schema
name: BirthData
properties_list:
- description: The individual's date of birth, in YYYY-MM-DD format.
  name: dateOfBirth
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-birth-data-schema.json
slug: legal-entity-birth-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-birth-data-schema.json\",\n  \"title\": \"BirthData\",\n  \"description\": \"BirthData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dateOfBirth\": {\n      \"description\": \"The individual's date of birth, in YYYY-MM-DD format.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-birth-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BirthData
---
