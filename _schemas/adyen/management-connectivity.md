---
description: Connectivity schema from Adyen API
layout: schema
name: Connectivity
properties_list:
- description: 'Indicates the status of the SIM card in the payment terminal. Can be updated and received only at terminal level, and only for models that support cellular connectivity. Possible values: * **ACTIVATED'
  name: simcardStatus
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-connectivity-schema.json
slug: management-connectivity
source_filename: management-connectivity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-connectivity-schema.json\",\n  \"title\": \"Connectivity\",\n  \"description\": \"Connectivity schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"simcardStatus\": {\n      \"description\": \"Indicates the status of the SIM card in the payment terminal. Can be updated and received only at terminal level, and only for models that support cellular connectivity.\\n\\nPossible values:\\n* **ACTIVATED**: the SIM card is activated. Cellular connectivity may still need to be enabled on the terminal itself, in the **Network** settings.\\n* **INVENTORY**: the SIM card is not activated. The terminal can't use cellular connectivity.\",\n      \"enum\": [\n        \"ACTIVATED\",\n        \"INVENTORY\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-connectivity-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Connectivity
---
