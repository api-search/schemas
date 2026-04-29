---
description: TotalDetails schema from Adyen API
layout: schema
name: TotalDetails
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-total-details-schema.json
slug: terminal-total-details
source_filename: terminal-total-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-total-details-schema.json\",\n  \"title\": \"TotalDetails\",\n  \"description\": \"TotalDetails schema from Adyen API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"OperatorID\",\n      \"POIID\",\n      \"SaleID\",\n      \"ShiftNumber\",\n      \"TotalsGroupID\"\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-total-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TotalDetails
---
