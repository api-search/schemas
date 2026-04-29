---
description: PayerList schema from Availity API
layout: schema
name: PayerList
properties_list:
- description: ''
  name: data
  type: array
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-payer-list-schema.json
slug: eligibility-payer-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-payer-list-schema.json\",\n  \"title\": \"PayerList\",\n  \"description\": \"PayerList schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"eligibilityUrl\": {\n            \"type\": \"string\"\n          },\n          \"supportedTransactions\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/eligibility-payer-list-schema.json
tags: []
title: PayerList
---
