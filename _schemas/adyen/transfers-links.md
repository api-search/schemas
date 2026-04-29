---
description: Links schema from Adyen API
layout: schema
name: Links
properties_list:
- description: Contains a link to the next page.
  name: next
  type: object
- description: Contains a link to the previous page.
  name: prev
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-links-schema.json
slug: transfers-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-links-schema.json\",\n  \"title\": \"Links\",\n  \"description\": \"Links schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next\": {\n      \"description\": \"Contains a link to the next page.\",\n      \"$ref\": \"#/components/schemas/Link\"\n    },\n    \"prev\": {\n      \"description\": \"Contains a link to the previous page.\",\n      \"$ref\": \"#/components/schemas/Link\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-links-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Links
---
