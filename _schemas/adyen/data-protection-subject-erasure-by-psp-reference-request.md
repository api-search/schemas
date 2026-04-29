---
description: SubjectErasureByPspReferenceRequest schema from Adyen API
layout: schema
name: SubjectErasureByPspReferenceRequest
properties_list:
- description: Set this to **true** if you want to delete shopper-related data, even if the shopper has an existing recurring transaction. This only deletes the shopper-related data for the specific payment, but doe
  name: forceErasure
  type: boolean
- description: Your merchant account
  name: merchantAccount
  type: string
- description: The PSP reference of the payment. We will delete all shopper-related data for this payment.
  name: pspReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/data-protection-subject-erasure-by-psp-reference-request-schema.json
slug: data-protection-subject-erasure-by-psp-reference-request
source_filename: data-protection-subject-erasure-by-psp-reference-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/data-protection-subject-erasure-by-psp-reference-request-schema.json\",\n  \"title\": \"SubjectErasureByPspReferenceRequest\",\n  \"description\": \"SubjectErasureByPspReferenceRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"forceErasure\": {\n      \"description\": \"Set this to **true** if you want to delete shopper-related data, even if the shopper has an existing recurring transaction. This only deletes the shopper-related data for the specific payment, but does not cancel the existing recurring transaction.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"Your merchant account\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The PSP reference of the payment. We will delete all shopper-related\
  \ data for this payment.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/data-protection-subject-erasure-by-psp-reference-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SubjectErasureByPspReferenceRequest
---
