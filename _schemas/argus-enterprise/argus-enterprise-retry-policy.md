---
description: RetryPolicy schema from ARGUS Enterprise API
layout: schema
name: RetryPolicy
properties_list:
- description: Maximum number of delivery retry attempts
  name: maxRetries
  type: integer
- description: Initial interval between retries in seconds
  name: retryIntervalSeconds
  type: integer
- description: Exponential backoff multiplier
  name: backoffMultiplier
  type: number
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-retry-policy-schema.json
slug: argus-enterprise-retry-policy
source_filename: argus-enterprise-retry-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-retry-policy-schema.json\",\n  \"title\": \"RetryPolicy\",\n  \"description\": \"RetryPolicy schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxRetries\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 10,\n      \"default\": 5,\n      \"description\": \"Maximum number of delivery retry attempts\"\n    },\n    \"retryIntervalSeconds\": {\n      \"type\": \"integer\",\n      \"minimum\": 10,\n      \"maximum\": 3600,\n      \"default\": 60,\n      \"description\": \"Initial interval between retries in seconds\"\n    },\n    \"backoffMultiplier\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"minimum\": 1.0,\n      \"maximum\": 5.0,\n      \"default\": 2.0,\n      \"description\": \"Exponential\
  \ backoff multiplier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-retry-policy-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: RetryPolicy
---
