---
description: ShopperInteractionDevice schema from Adyen API
layout: schema
name: ShopperInteractionDevice
properties_list:
- description: Locale on the shopper interaction device.
  name: locale
  type: string
- description: Operating system running on the shopper interaction device.
  name: os
  type: string
- description: Version of the operating system on the shopper interaction device.
  name: osVersion
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-shopper-interaction-device-schema.json
slug: checkout-shopper-interaction-device
source_filename: checkout-shopper-interaction-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-shopper-interaction-device-schema.json\",\n  \"title\": \"ShopperInteractionDevice\",\n  \"description\": \"ShopperInteractionDevice schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locale\": {\n      \"description\": \"Locale on the shopper interaction device.\",\n      \"type\": \"string\"\n    },\n    \"os\": {\n      \"description\": \"Operating system running on the shopper interaction device.\",\n      \"type\": \"string\"\n    },\n    \"osVersion\": {\n      \"description\": \"Version of the operating system on the shopper interaction device.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-shopper-interaction-device-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ShopperInteractionDevice
---
