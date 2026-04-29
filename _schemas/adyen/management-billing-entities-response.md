---
description: BillingEntitiesResponse schema from Adyen API
layout: schema
name: BillingEntitiesResponse
properties_list:
- description: List of legal entities that can be used for the billing of orders.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-billing-entities-response-schema.json
slug: management-billing-entities-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-billing-entities-response-schema.json\",\n  \"title\": \"BillingEntitiesResponse\",\n  \"description\": \"BillingEntitiesResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"List of legal entities that can be used for the billing of orders.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BillingEntity\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-billing-entities-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BillingEntitiesResponse
---
