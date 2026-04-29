---
description: MealVoucherFRInfo schema from Adyen API
layout: schema
name: MealVoucherFRInfo
properties_list:
- description: 'Meal Voucher conecsId. Format: digits only'
  name: conecsId
  type: string
- description: 'Meal Voucher siret. Format: 14 digits.'
  name: siret
  type: string
- description: 'The list of additional payment methods. Allowed values: **mealVoucher_FR_edenred**, **mealVoucher_FR_groupeup**, **mealVoucher_FR_natixis**, **mealVoucher_FR_sodexo**.'
  name: subTypes
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-meal-voucher-fr-info-schema.json
slug: management-meal-voucher-fr-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-meal-voucher-fr-info-schema.json\",\n  \"title\": \"MealVoucherFRInfo\",\n  \"description\": \"MealVoucherFRInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conecsId\": {\n      \"description\": \"Meal Voucher conecsId. Format: digits only\",\n      \"type\": \"string\"\n    },\n    \"siret\": {\n      \"description\": \"Meal Voucher siret. Format: 14 digits.\",\n      \"maxLength\": 14,\n      \"minLength\": 14,\n      \"type\": \"string\"\n    },\n    \"subTypes\": {\n      \"description\": \"The list of additional payment methods. Allowed values: **mealVoucher_FR_edenred**, **mealVoucher_FR_groupeup**, **mealVoucher_FR_natixis**, **mealVoucher_FR_sodexo**.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\"\
  : [\n    \"siret\",\n    \"conecsId\",\n    \"subTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-meal-voucher-fr-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MealVoucherFRInfo
---
