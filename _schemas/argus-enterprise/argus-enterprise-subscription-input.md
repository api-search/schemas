---
description: SubscriptionInput schema from ARGUS Enterprise API
layout: schema
name: SubscriptionInput
properties_list:
- description: HTTPS endpoint URL for webhook delivery
  name: url
  type: string
- description: ''
  name: eventTypes
  type: array
- description: ''
  name: description
  type: string
- description: ''
  name: retryPolicy
  type: object
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-subscription-input-schema.json
slug: argus-enterprise-subscription-input
source_filename: argus-enterprise-subscription-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-subscription-input-schema.json\",\n  \"title\": \"SubscriptionInput\",\n  \"description\": \"SubscriptionInput schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS endpoint URL for webhook delivery\"\n    },\n    \"eventTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"property.created\",\n          \"property.updated\",\n          \"property.deleted\",\n          \"valuation.created\",\n          \"valuation.updated\",\n          \"lease.created\",\n          \"lease.updated\",\n          \"lease.expired\",\n          \"portfolio.created\",\n          \"portfolio.updated\",\n   \
  \       \"portfolio.deleted\",\n          \"report.completed\",\n          \"report.failed\",\n          \"cashflow.updated\",\n          \"tenant.created\",\n          \"tenant.updated\"\n        ]\n      },\n      \"minItems\": 1\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"retryPolicy\": {\n      \"$ref\": \"#/components/schemas/RetryPolicy\"\n    }\n  },\n  \"required\": [\n    \"url\",\n    \"eventTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-subscription-input-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: SubscriptionInput
---
