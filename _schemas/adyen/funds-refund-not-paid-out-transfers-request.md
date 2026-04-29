---
description: RefundNotPaidOutTransfersRequest schema from Adyen API
layout: schema
name: RefundNotPaidOutTransfersRequest
properties_list:
- description: The code of the account from which to perform the refund(s).
  name: accountCode
  type: string
- description: The code of the Account Holder which owns the account from which to perform the refund(s).
  name: accountHolderCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-refund-not-paid-out-transfers-request-schema.json
slug: funds-refund-not-paid-out-transfers-request
source_filename: funds-refund-not-paid-out-transfers-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-refund-not-paid-out-transfers-request-schema.json\",\n  \"title\": \"RefundNotPaidOutTransfersRequest\",\n  \"description\": \"RefundNotPaidOutTransfersRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountCode\": {\n      \"description\": \"The code of the account from which to perform the refund(s).\",\n      \"type\": \"string\"\n    },\n    \"accountHolderCode\": {\n      \"description\": \"The code of the Account Holder which owns the account from which to perform the refund(s).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"accountHolderCode\",\n    \"accountCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-refund-not-paid-out-transfers-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RefundNotPaidOutTransfersRequest
---
