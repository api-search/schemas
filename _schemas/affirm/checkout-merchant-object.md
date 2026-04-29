---
description: Merchant-specific configuration for the checkout, including callback URLs and the public API key.
layout: schema
name: MerchantObject
properties_list:
- description: The merchant's public API key. Required for checkout and store endpoints when submitting from a server context.
  name: public_api_key
  type: string
- description: The URL the customer is redirected to after successfully completing the Affirm checkout flow. A checkout_token is delivered to this URL via POST or GET depending on user_confirmation_url_action.
  name: user_confirmation_url
  type: string
- description: The URL the customer is redirected to if they cancel or abandon the Affirm checkout flow.
  name: user_cancel_url
  type: string
- description: Determines how the checkout_token is delivered to the user_confirmation_url. "POST" sends it as a form body field; "GET" appends it as a query parameter.
  name: user_confirmation_url_action
  type: string
- description: The merchant's display name, shown to customers during checkout.
  name: name
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/checkout-merchant-object-schema.json
slug: checkout-merchant-object
source_filename: checkout-merchant-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-merchant-object-schema.json\",\n  \"title\": \"MerchantObject\",\n  \"description\": \"Merchant-specific configuration for the checkout, including callback URLs and the public API key.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"public_api_key\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's public API key. Required for checkout and store endpoints when submitting from a server context.\",\n      \"example\": \"abc123def456abc123def456abc123de\"\n    },\n    \"user_confirmation_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL the customer is redirected to after successfully completing the Affirm checkout flow. A checkout_token is delivered to this URL via POST or GET depending on user_confirmation_url_action.\",\n\
  \      \"example\": \"https://example.com/path\"\n    },\n    \"user_cancel_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL the customer is redirected to if they cancel or abandon the Affirm checkout flow.\",\n      \"example\": \"https://example.com/path\"\n    },\n    \"user_confirmation_url_action\": {\n      \"type\": \"string\",\n      \"description\": \"Determines how the checkout_token is delivered to the user_confirmation_url. \\\"POST\\\" sends it as a form body field; \\\"GET\\\" appends it as a query parameter.\",\n      \"enum\": [\n        \"POST\",\n        \"GET\"\n      ],\n      \"default\": \"POST\",\n      \"example\": \"POST\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's display name, shown to customers during checkout.\",\n      \"example\": \"Example Merchant\"\n    }\n  },\n  \"required\": [\n    \"user_confirmation_url\",\n    \"user_cancel_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/checkout-merchant-object-schema.json
tags: []
title: MerchantObject
---
