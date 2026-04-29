---
description: ReceiptOptions schema from Adyen API
layout: schema
name: ReceiptOptions
properties_list:
- description: The receipt logo converted to a Base64-encoded string. The image must be a .bmp file of < 256 KB, dimensions 240 (H) x 384 (W) px.
  name: logo
  type: string
- description: Indicates whether a screen appears asking if you want to print the shopper receipt.
  name: promptBeforePrinting
  type: boolean
- description: 'Data to print on the receipt as a QR code. This can include static text and the following variables: - `${merchantreference}`: the merchant reference of the transaction. - `${pspreference}`: the PSP r'
  name: qrCodeData
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-receipt-options-schema.json
slug: management-receipt-options
source_filename: management-receipt-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-receipt-options-schema.json\",\n  \"title\": \"ReceiptOptions\",\n  \"description\": \"ReceiptOptions schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logo\": {\n      \"description\": \"The receipt logo converted to a Base64-encoded string. The image must be a .bmp file of < 256 KB, dimensions 240 (H) x 384 (W) px.\",\n      \"maxLength\": 350000,\n      \"type\": \"string\"\n    },\n    \"promptBeforePrinting\": {\n      \"description\": \"Indicates whether a screen appears asking if you want to print the shopper receipt.\",\n      \"type\": \"boolean\"\n    },\n    \"qrCodeData\": {\n      \"description\": \"Data to print on the receipt as a QR code. This can include static text and the following variables:\\n\\n- `${merchantreference}`: the merchant reference of the transaction.\\\
  n- `${pspreference}`: the PSP reference of the transaction.\\n\\n For example, **http://www.example.com/order/${pspreference}/${merchantreference}**.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-receipt-options-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReceiptOptions
---
