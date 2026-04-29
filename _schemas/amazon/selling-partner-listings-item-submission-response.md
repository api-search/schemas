---
description: ListingsItemSubmissionResponse schema from Amazon Selling Partner API
layout: schema
name: ListingsItemSubmissionResponse
properties_list:
- description: ''
  name: sku
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: submissionId
  type: string
- description: ''
  name: issues
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-listings-item-submission-response-schema.json
slug: selling-partner-listings-item-submission-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"sku\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACCEPTED\",\n        \"INVALID\"\n      ]\n    },\n    \"submissionId\": {\n      \"type\": \"string\"\n    },\n    \"issues\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListingsItemSubmissionResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-listings-item-submission-response-schema.json\",\n  \"description\": \"ListingsItemSubmissionResponse schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-listings-item-submission-response-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: ListingsItemSubmissionResponse
---
