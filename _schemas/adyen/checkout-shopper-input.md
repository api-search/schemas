---
description: ShopperInput schema from Adyen API
layout: schema
name: ShopperInput
properties_list:
- description: 'Specifies visibility of billing address fields. Permitted values: * editable * hidden * readOnly'
  name: billingAddress
  type: string
- description: 'Specifies visibility of delivery address fields. Permitted values: * editable * hidden * readOnly'
  name: deliveryAddress
  type: string
- description: 'Specifies visibility of personal details. Permitted values: * editable * hidden * readOnly'
  name: personalDetails
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-shopper-input-schema.json
slug: checkout-shopper-input
source_filename: checkout-shopper-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-shopper-input-schema.json\",\n  \"title\": \"ShopperInput\",\n  \"description\": \"ShopperInput schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingAddress\": {\n      \"description\": \"Specifies visibility of billing address fields.\\n\\nPermitted values:\\n* editable\\n* hidden\\n* readOnly\",\n      \"enum\": [\n        \"editable\",\n        \"hidden\",\n        \"readOnly\"\n      ],\n      \"type\": \"string\"\n    },\n    \"deliveryAddress\": {\n      \"description\": \"Specifies visibility of delivery address fields.\\n\\nPermitted values:\\n* editable\\n* hidden\\n* readOnly\",\n      \"enum\": [\n        \"editable\",\n        \"hidden\",\n        \"readOnly\"\n      ],\n      \"type\": \"string\"\n    },\n    \"personalDetails\": {\n      \"description\": \"\
  Specifies visibility of personal details.\\n\\nPermitted values:\\n* editable\\n* hidden\\n* readOnly\",\n      \"enum\": [\n        \"editable\",\n        \"hidden\",\n        \"readOnly\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-shopper-input-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ShopperInput
---
