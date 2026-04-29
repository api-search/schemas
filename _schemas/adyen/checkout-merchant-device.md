---
description: MerchantDevice schema from Adyen API
layout: schema
name: MerchantDevice
properties_list:
- description: Operating system running on the merchant device.
  name: os
  type: string
- description: Version of the operating system on the merchant device.
  name: osVersion
  type: string
- description: Merchant device reference.
  name: reference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-merchant-device-schema.json
slug: checkout-merchant-device
source_filename: checkout-merchant-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-merchant-device-schema.json\",\n  \"title\": \"MerchantDevice\",\n  \"description\": \"MerchantDevice schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"os\": {\n      \"description\": \"Operating system running on the merchant device.\",\n      \"type\": \"string\"\n    },\n    \"osVersion\": {\n      \"description\": \"Version of the operating system on the merchant device.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Merchant device reference.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-merchant-device-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MerchantDevice
---
