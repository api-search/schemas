---
description: ModificationResult schema from Adyen API
layout: schema
name: ModificationResult
properties_list:
- description: This field contains additional data, which may be returned in a particular modification response.
  name: additionalData
  type: object
- description: Adyen's 16-character string reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.
  name: pspReference
  type: string
- description: Indicates if the modification request has been received for processing.
  name: response
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-modification-result-schema.json
slug: payments-modification-result
source_filename: payments-modification-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-modification-result-schema.json\",\n  \"title\": \"ModificationResult\",\n  \"description\": \"ModificationResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be returned in a particular modification response.\",\n      \"type\": \"object\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character string reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.\",\n      \"type\": \"string\"\n    },\n    \"response\": {\n      \"description\": \"Indicates if the modification request has been received for processing.\"\
  ,\n      \"enum\": [\n        \"[capture-received]\",\n        \"[cancel-received]\",\n        \"[refund-received]\",\n        \"[cancelOrRefund-received]\",\n        \"[adjustAuthorisation-received]\",\n        \"[donation-received]\",\n        \"[technical-cancel-received]\",\n        \"[voidPendingRefund-received]\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"response\",\n    \"pspReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-modification-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ModificationResult
---
