---
description: BinDetail schema from Adyen API
layout: schema
name: BinDetail
properties_list:
- description: The country where the card was issued.
  name: issuerCountry
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-bin-detail-schema.json
slug: binlookup-bin-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-bin-detail-schema.json\",\n  \"title\": \"BinDetail\",\n  \"description\": \"BinDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"issuerCountry\": {\n      \"description\": \"The country where the card was issued.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-bin-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BinDetail
---
