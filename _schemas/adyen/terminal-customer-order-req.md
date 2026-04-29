---
description: CustomerOrderReq schema from Adyen API
layout: schema
name: CustomerOrderReq
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-customer-order-req-schema.json
slug: terminal-customer-order-req
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-customer-order-req-schema.json\",\n  \"title\": \"CustomerOrderReq\",\n  \"description\": \"CustomerOrderReq schema from Adyen API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"Both\",\n      \"Closed\",\n      \"Open\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-customer-order-req-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CustomerOrderReq
---
