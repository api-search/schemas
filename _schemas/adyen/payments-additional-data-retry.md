---
description: AdditionalDataRetry schema from Adyen API
layout: schema
name: AdditionalDataRetry
properties_list:
- description: The number of times the transaction (not order) has been retried between different payment service providers. For instance, the `chainAttemptNumber` set to 2 means that this transaction has been recen
  name: retry.chainAttemptNumber
  type: string
- description: The index of the attempt to bill a particular order, which is identified by the `merchantOrderReference` field. For example, if a recurring transaction fails and is retried one day later, then the ord
  name: retry.orderAttemptNumber
  type: string
- description: 'The Boolean value indicating whether Adyen should skip or retry this transaction, if possible. > If you submit `retry.chainAttemptNumber`, `retry.orderAttemptNumber`, and `retry.skipRetry` values, we '
  name: retry.skipRetry
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-additional-data-retry-schema.json
slug: payments-additional-data-retry
source_filename: payments-additional-data-retry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-additional-data-retry-schema.json\",\n  \"title\": \"AdditionalDataRetry\",\n  \"description\": \"AdditionalDataRetry schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"retry.chainAttemptNumber\": {\n      \"description\": \"The number of times the transaction (not order) has been retried between different payment service providers. For instance, the `chainAttemptNumber` set to 2 means that this transaction has been recently tried on another provider before being sent to Adyen.\\n\\n> If you submit `retry.chainAttemptNumber`, `retry.orderAttemptNumber`, and `retry.skipRetry` values, we also recommend you provide the `merchantOrderReference` to facilitate linking payment attempts together.\",\n      \"type\": \"string\"\n    },\n    \"retry.orderAttemptNumber\": {\n      \"description\"\
  : \"The index of the attempt to bill a particular order, which is identified by the `merchantOrderReference` field. For example, if a recurring transaction fails and is retried one day later, then the order number for these attempts would be 1 and 2, respectively.\\n\\n> If you submit `retry.chainAttemptNumber`, `retry.orderAttemptNumber`, and `retry.skipRetry` values, we also recommend you provide the `merchantOrderReference` to facilitate linking payment attempts together.\",\n      \"type\": \"string\"\n    },\n    \"retry.skipRetry\": {\n      \"description\": \"The Boolean value indicating whether Adyen should skip or retry this transaction, if possible.\\n\\n> If you submit `retry.chainAttemptNumber`, `retry.orderAttemptNumber`, and `retry.skipRetry` values, we also recommend you provide the `merchantOrderReference` to facilitate linking payment attempts together.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-additional-data-retry-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataRetry
---
