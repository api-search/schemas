---
description: Represents a discount applied to the checkout.
layout: schema
name: DiscountObject
properties_list:
- description: The discount amount in cents.
  name: discount_amount
  type: integer
- description: Customer-facing name or description of the discount.
  name: discount_display_name
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-discount-object-schema.json
slug: checkout-discount-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-discount-object-schema.json\",\n  \"title\": \"DiscountObject\",\n  \"description\": \"Represents a discount applied to the checkout.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"discount_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The discount amount in cents.\",\n      \"minimum\": 0,\n      \"example\": 1\n    },\n    \"discount_display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-facing name or description of the discount.\",\n      \"example\": \"Example Merchant\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-discount-object-schema.json
tags: []
title: DiscountObject
---
