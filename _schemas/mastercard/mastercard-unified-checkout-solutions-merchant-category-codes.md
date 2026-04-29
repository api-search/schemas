---
description: 'Object for the array of Merchant Category Codes (MCC) that the Merchant processes transactions under, and is used for risk-scoring transactions by the issuer. All MCC codes that will be processed by a DPA should be provided here (typically, this will be a single item). An MCC is a four-character code assigned by Mastercard to the Merchant that indicates the type of business, service, or product provided by the Merchant. Note: MCC''s may be assigned differently across payment networks. To avoid errors, be sure to use your assigned Mastercard MCC. This code is required for 3-D Secure (3DS) and risk profiling. If the Merchant has more than one MCC, the code most relevant to their business should be used.'
layout: schema
name: merchantCategoryCodes
properties_list: []
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-unified-checkout-solutions-merchant-category-codes-schema.json
slug: mastercard-unified-checkout-solutions-merchant-category-codes
source_filename: mastercard-unified-checkout-solutions-merchant-category-codes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"merchantCategoryCodes\",\n  \"type\": \"array\",\n  \"description\": \"Object for the array of Merchant Category Codes (MCC) that the Merchant processes transactions under, and is used for risk-scoring transactions by the issuer. All MCC codes that will be processed by a DPA should be provided here (typically, this will be a single item).\\n\\nAn MCC is a four-character code assigned by Mastercard to the Merchant that indicates the type of business, service, or product provided by the Merchant.\\n\\nNote: MCC's may be assigned differently across payment networks. To avoid errors, be sure to use your assigned Mastercard MCC. This code is required for 3-D Secure (3DS) and risk profiling. If the Merchant has more than one MCC, the code most relevant to their business should be used.\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-unified-checkout-solutions-merchant-category-codes-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: merchantCategoryCodes
---
