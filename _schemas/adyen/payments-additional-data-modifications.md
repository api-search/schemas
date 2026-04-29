---
description: AdditionalDataModifications schema from Adyen API
layout: schema
name: AdditionalDataModifications
properties_list:
- description: This is the installment option selected by the shopper. It is required only if specified by the user.
  name: installmentPaymentData.selectedInstallmentOption
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-additional-data-modifications-schema.json
slug: payments-additional-data-modifications
source_filename: payments-additional-data-modifications-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-additional-data-modifications-schema.json\",\n  \"title\": \"AdditionalDataModifications\",\n  \"description\": \"AdditionalDataModifications schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"installmentPaymentData.selectedInstallmentOption\": {\n      \"description\": \"This is the installment option selected by the shopper. It is required only if specified by the user.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-additional-data-modifications-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataModifications
---
