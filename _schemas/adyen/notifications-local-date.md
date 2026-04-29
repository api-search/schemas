---
description: LocalDate schema from Adyen API
layout: schema
name: LocalDate
properties_list:
- description: ''
  name: month
  type: integer
- description: ''
  name: year
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-local-date-schema.json
slug: notifications-local-date
source_filename: notifications-local-date-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-local-date-schema.json\",\n  \"title\": \"LocalDate\",\n  \"description\": \"LocalDate schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"month\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"year\": {\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-local-date-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LocalDate
---
