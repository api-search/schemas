---
description: ''
layout: schema
name: CategoryPurpose
properties_list:
- description: Use-case (represented via category purpose codes) supported by the DSP. *Refer to Codes and Formats section for more details.
  name: categoryPurpose
  type: string
- description: List of features (represented via featureList codes) supported for each categoryPurpose by the DSP. *Refer to Codes and Formats section for more details.
  name: featureList
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-category-purpose-schema.json
slug: mastercard-account-to-account-commerce-for-creditor-service-providers-category-purpose
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CategoryPurpose\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"categoryPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"Use-case (represented via category purpose codes) supported by the DSP.  *Refer to Codes and Formats section for more details.\"\n    },\n    \"featureList\": {\n      \"type\": \"array\",\n      \"description\": \"List of features (represented via featureList codes) supported for each categoryPurpose by the DSP.  *Refer to Codes and Formats section for more details.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-account-to-account-commerce-for-creditor-service-providers-category-purpose-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: CategoryPurpose
---
