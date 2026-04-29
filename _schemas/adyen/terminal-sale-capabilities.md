---
description: SaleCapabilities schema from Adyen API
layout: schema
name: SaleCapabilities
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-sale-capabilities-schema.json
slug: terminal-sale-capabilities
source_filename: terminal-sale-capabilities-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-capabilities-schema.json\",\n  \"title\": \"SaleCapabilities\",\n  \"description\": \"SaleCapabilities schema from Adyen API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"CashierDisplay\",\n      \"CashierError\",\n      \"CashierInput\",\n      \"CashierStatus\",\n      \"CustomerAssistance\",\n      \"CustomerDisplay\",\n      \"CustomerError\",\n      \"CustomerInput\",\n      \"EMVContactless\",\n      \"ICC\",\n      \"MagStripe\",\n      \"POIReplication\",\n      \"PrinterDocument\",\n      \"PrinterReceipt\",\n      \"PrinterVoucher\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-sale-capabilities-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SaleCapabilities
---
