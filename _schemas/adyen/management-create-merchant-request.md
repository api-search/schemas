---
description: CreateMerchantRequest schema from Adyen API
layout: schema
name: CreateMerchantRequest
properties_list:
- description: The unique identifier of the [business line](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/businessLines). Required for an Adyen for Platforms Manage integration.
  name: businessLineId
  type: string
- description: The unique identifier of the company account.
  name: companyId
  type: string
- description: Your description for the merchant account, maximum 300 characters.
  name: description
  type: string
- description: The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities). Required for an Adyen for Platforms Manage integration.
  name: legalEntityId
  type: string
- description: Sets the pricing plan for the merchant account. Required for an Adyen for Platforms Manage integration. Your Adyen contact will provide the values that you can use.
  name: pricingPlan
  type: string
- description: Your reference for the merchant account. To make this reference the unique identifier of the merchant account, your Adyen contact can set up a template on your company account. The template can have 6
  name: reference
  type: string
- description: List of sales channels that the merchant will process payments with
  name: salesChannels
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-create-merchant-request-schema.json
slug: management-create-merchant-request
source_filename: management-create-merchant-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-merchant-request-schema.json\",\n  \"title\": \"CreateMerchantRequest\",\n  \"description\": \"CreateMerchantRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"businessLineId\": {\n      \"description\": \"The unique identifier of the [business line](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/businessLines). Required for an Adyen for Platforms Manage integration.\",\n      \"type\": \"string\"\n    },\n    \"companyId\": {\n      \"description\": \"The unique identifier of the company account.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the merchant account, maximum 300 characters.\",\n      \"maxLength\": 300,\n      \"type\": \"string\"\n    },\n    \"legalEntityId\": {\n  \
  \    \"description\": \"The unique identifier of the [legal entity](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/legalEntities). Required for an Adyen for Platforms Manage integration.\",\n      \"type\": \"string\"\n    },\n    \"pricingPlan\": {\n      \"description\": \"Sets the pricing plan for the merchant account. Required for an Adyen for Platforms Manage integration. Your Adyen contact will provide the values that you can use.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your reference for the merchant account. To make this reference the unique identifier of the merchant account, your Adyen contact can set up a template on your company account. The template can have 6 to 255 characters with upper- and lower-case letters, underscores, and numbers. When your company account has a template, then the `reference` is required and must be unique within the company account.\",\n      \"type\": \"string\"\n    },\n    \"salesChannels\"\
  : {\n      \"description\": \"List of sales channels that the merchant will process payments with\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"companyId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-merchant-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateMerchantRequest
---
