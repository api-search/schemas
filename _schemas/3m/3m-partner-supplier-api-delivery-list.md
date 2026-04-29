---
description: List of delivery records
layout: schema
name: DeliveryList
properties_list:
- description: Array of delivery records
  name: deliveries
  type: array
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-delivery-list-schema.json
slug: 3m-partner-supplier-api-delivery-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-delivery-list-schema.json\",\n  \"title\": \"DeliveryList\",\n  \"description\": \"List of delivery records\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deliveries\": {\n      \"type\": \"array\",\n      \"description\": \"Array of delivery records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Delivery\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-delivery-list-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: DeliveryList
---
