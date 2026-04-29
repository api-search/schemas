---
description: A registered consumer with consent for credit data access.
layout: schema
name: Consumer
properties_list:
- description: Unique identifier for the consumer.
  name: consumer_id
  type: string
- description: Consumer's first name.
  name: first_name
  type: string
- description: Consumer's last name.
  name: last_name
  type: string
- description: Consumer's email address.
  name: email
  type: string
- description: Consumer account status.
  name: status
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Bloom Credit
provider_slug: bloom-credit
schema_file: json-schema/bloom-credit-consumer-schema.json
slug: bloom-credit-consumer
source_filename: bloom-credit-consumer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bloom-credit/main/json-schema/bloom-credit-consumer-schema.json\",\n  \"title\": \"Consumer\",\n  \"description\": \"A registered consumer with consent for credit data access.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"consumer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the consumer.\",\n      \"example\": \"cns_8f7d3a2b1c4e5f6a\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer's first name.\",\n      \"example\": \"Jane\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer's last name.\",\n      \"example\": \"Smith\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Consumer's email address.\",\n      \"example\": \"jane.smith@example.com\"\n\
  \    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer account status.\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\", \"PENDING\"],\n      \"example\": \"ACTIVE\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:00:00Z\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloom-credit/refs/heads/main/json-schema/bloom-credit-consumer-schema.json
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
title: Consumer
---
