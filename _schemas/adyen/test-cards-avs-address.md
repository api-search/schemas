---
description: AvsAddress schema from Adyen API
layout: schema
name: AvsAddress
properties_list:
- description: 'The street and house number of the address. Example: 1 Infinite Loop, Cupertino.'
  name: streetAddress
  type: string
- description: 'The zip or post code of the address. Example: CA 95014'
  name: zip
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/test-cards-avs-address-schema.json
slug: test-cards-avs-address
source_filename: test-cards-avs-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-avs-address-schema.json\",\n  \"title\": \"AvsAddress\",\n  \"description\": \"AvsAddress schema from Adyen API\",\n  \"properties\": {\n    \"streetAddress\": {\n      \"description\": \"The street and house number of the address.\\n\\nExample: 1 Infinite Loop, Cupertino.\",\n      \"type\": \"string\"\n    },\n    \"zip\": {\n      \"description\": \"The zip or post code of the address.\\n\\nExample: CA 95014\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"streetAddress\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/test-cards-avs-address-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AvsAddress
---
