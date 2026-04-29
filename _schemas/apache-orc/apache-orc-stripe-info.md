---
description: StripeInfo schema from Apache ORC
layout: schema
name: StripeInfo
properties_list:
- description: ''
  name: stripeIndex
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: length
  type: integer
- description: ''
  name: rowCount
  type: integer
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-stripe-info-schema.json
slug: apache-orc-stripe-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-stripe-info-schema.json\",\n  \"title\": \"StripeInfo\",\n  \"description\": \"StripeInfo schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stripeIndex\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"example\": 3\n    },\n    \"length\": {\n      \"type\": \"integer\",\n      \"example\": 1048576\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"example\": 100000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-stripe-info-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: StripeInfo
---
