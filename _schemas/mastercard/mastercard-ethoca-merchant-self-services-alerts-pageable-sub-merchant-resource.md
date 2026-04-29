---
description: Pageable response containing sub-merchants with their details
layout: schema
name: AlertsPageableSubMerchantResource
properties_list:
- description: List of sub-merchants with all details
  name: subMerchants
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-alerts-pageable-sub-merchant-resource-schema.json
slug: mastercard-ethoca-merchant-self-services-alerts-pageable-sub-merchant-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlertsPageableSubMerchantResource\",\n  \"type\": \"object\",\n  \"description\": \"Pageable response containing sub-merchants with their details\",\n  \"properties\": {\n    \"subMerchants\": {\n      \"type\": \"array\",\n      \"description\": \"List of sub-merchants with all details\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-alerts-pageable-sub-merchant-resource-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AlertsPageableSubMerchantResource
---
