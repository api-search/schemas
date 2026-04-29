---
description: TransferRouteResponse schema from Adyen API
layout: schema
name: TransferRouteResponse
properties_list:
- description: List of available priorities for a transfer, along with requirements. Use this information to initiate a transfer.
  name: transferRoutes
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transfer-route-response-schema.json
slug: configuration-transfer-route-response
source_filename: configuration-transfer-route-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transfer-route-response-schema.json\",\n  \"title\": \"TransferRouteResponse\",\n  \"description\": \"TransferRouteResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transferRoutes\": {\n      \"description\": \"List of available priorities for a transfer, along with requirements. Use this information to initiate a transfer.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TransferRoute\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transfer-route-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferRouteResponse
---
