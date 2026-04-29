---
description: SessionResultResponse schema from Adyen API
layout: schema
name: SessionResultResponse
properties_list:
- description: A unique identifier of the session.
  name: id
  type: string
- description: 'The status of the session. The status included in the response doesn''t get updated. Don''t make the request again to check for payment status updates. Possible values: * **completed** – The shopper com'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-session-result-response-schema.json
slug: checkout-session-result-response
source_filename: checkout-session-result-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-session-result-response-schema.json\",\n  \"title\": \"SessionResultResponse\",\n  \"description\": \"SessionResultResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"A unique identifier of the session.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the session. The status included in the response doesn't get updated. Don't make the request again to check for payment status updates.\\n\\nPossible values:\\n\\n         * **completed** \\u2013 The shopper completed the payment. This means that the payment was authorized.\\n         * **paymentPending** \\u2013 The shopper is in the process of making the payment. This applies to payment methods with an asynchronous flow.\\n         * **refused**\
  \ \\u2013 The session has been refused, due to too many refused payment attempts. Shoppers can no longer complete the payment with this session.\\n         * **canceled** \\u2013 The shopper canceled the payment.\\n         * **active** \\u2013 The session is still active and can be paid.\\n         * **expired** \\u2013 The session expired (default: 1 hour after session creation). Shoppers can no longer complete the payment with this session.\\n\",\n      \"enum\": [\n        \"active\",\n        \"canceled\",\n        \"completed\",\n        \"expired\",\n        \"paymentPending\",\n        \"refused\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-session-result-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SessionResultResponse
---
