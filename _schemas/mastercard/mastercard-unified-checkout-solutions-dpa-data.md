---
description: ''
layout: schema
name: DpaData
properties_list:
- description: Legal name of Merchant (which may differ from dpaPresentationName).
  name: dpaName
  type: string
- description: The name of the Merchant that the Cardholder will see when checking out with the Digital Payment Application (DPA).
  name: dpaPresentationName
  type: string
- description: Digital Payment Application (DPA) identifier. This field may contain the DPA website URI, a mobile application identifier, or another unique identifier (UUID, URL, APK package name, etc.).
  name: dpaUri
  type: string
- description: Website or URL where the payment experience is placed on the checkout page.
  name: originDomains
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-unified-checkout-solutions-dpa-data-schema.json
slug: mastercard-unified-checkout-solutions-dpa-data
source_filename: mastercard-unified-checkout-solutions-dpa-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DpaData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dpaName\": {\n      \"type\": \"string\",\n      \"description\": \"Legal name of Merchant (which may differ from dpaPresentationName).\"\n    },\n    \"dpaPresentationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Merchant that the Cardholder will see when checking out with the Digital Payment Application (DPA).\"\n    },\n    \"dpaUri\": {\n      \"type\": \"string\",\n      \"description\": \"Digital Payment Application (DPA) identifier. This field may contain the DPA website URI, a mobile application identifier, or another unique identifier (UUID, URL, APK package name, etc.).\"\n    },\n    \"originDomains\": {\n      \"type\": \"array\",\n      \"description\": \"Website or URL where the payment experience is placed on the checkout page.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-unified-checkout-solutions-dpa-data-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DpaData
---
