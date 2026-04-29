---
description: UpdateNetworkTokenRequest schema from Adyen API
layout: schema
name: UpdateNetworkTokenRequest
properties_list:
- description: 'The new status of the network token. Possible values: **active**, **suspended**, **closed**. The **closed** status is final and cannot be changed.'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-update-network-token-request-schema.json
slug: configuration-update-network-token-request
source_filename: configuration-update-network-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-update-network-token-request-schema.json\",\n  \"title\": \"UpdateNetworkTokenRequest\",\n  \"description\": \"UpdateNetworkTokenRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"description\": \"The new status of the network token. Possible values: **active**, **suspended**, **closed**. The **closed** status is final and cannot be changed.\",\n      \"enum\": [\n        \"active\",\n        \"suspended\",\n        \"closed\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-update-network-token-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpdateNetworkTokenRequest
---
