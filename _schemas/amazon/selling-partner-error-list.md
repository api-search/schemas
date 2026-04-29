---
description: ErrorList schema from Amazon Selling Partner API
layout: schema
name: ErrorList
properties_list:
- description: ''
  name: errors
  type: array
provider_name: Amazon
provider_slug: amazon
schema_file: json-schema/selling-partner-error-list-schema.json
slug: selling-partner-error-list
source_filename: selling-partner-error-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Error\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorList\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-error-list-schema.json\",\n  \"description\": \"ErrorList schema from Amazon Selling Partner API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/json-schema/selling-partner-error-list-schema.json
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
title: ErrorList
---
