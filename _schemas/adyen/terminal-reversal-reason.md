---
description: Reason of the payment or loyalty reversal..
layout: schema
name: ReversalReason
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-reversal-reason-schema.json
slug: terminal-reversal-reason
source_filename: terminal-reversal-reason-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reversal-reason-schema.json\",\n  \"title\": \"ReversalReason\",\n  \"description\": \"Reason of the payment or loyalty reversal..\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CustCancel\",\n    \"Malfunction\",\n    \"MerchantCancel\",\n    \"Unable2Compl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reversal-reason-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReversalReason
---
