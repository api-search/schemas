---
description: POICapabilities schema from Adyen API
layout: schema
name: POICapabilities
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-poi-capabilities-schema.json
slug: terminal-poi-capabilities
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-capabilities-schema.json\",\n  \"title\": \"POICapabilities\",\n  \"description\": \"POICapabilities schema from Adyen API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"CashHandling\",\n      \"CashierDisplay\",\n      \"CashierError\",\n      \"CashierInput\",\n      \"CustomerDisplay\",\n      \"CustomerError\",\n      \"CustomerInput\",\n      \"EMVContactless\",\n      \"ICC\",\n      \"MagStripe\",\n      \"PrinterDocument\",\n      \"PrinterReceipt\",\n      \"PrinterVoucher\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-capabilities-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: POICapabilities
---
