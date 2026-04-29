---
description: WebData schema from Adyen API
layout: schema
name: WebData
properties_list:
- description: The URL of the website or the app store URL.
  name: webAddress
  type: string
- description: The unique identifier of the web address.
  name: webAddressId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-web-data-schema.json
slug: legal-entity-web-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-web-data-schema.json\",\n  \"title\": \"WebData\",\n  \"description\": \"WebData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webAddress\": {\n      \"description\": \"The URL of the website or the app store URL.\",\n      \"type\": \"string\"\n    },\n    \"webAddressId\": {\n      \"description\": \"The unique identifier of the web address.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-web-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: WebData
---
