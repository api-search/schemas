---
description: Subscription schema from ARGUS Enterprise API
layout: schema
name: Subscription
properties_list:
- description: Unique subscription identifier
  name: id
  type: string
- description: HTTPS endpoint URL for webhook delivery
  name: url
  type: string
- description: Event types this subscription receives
  name: eventTypes
  type: array
- description: Current subscription status
  name: status
  type: string
- description: Shared secret for HMAC-SHA256 signature verification of webhook payloads (only returned on creation)
  name: secret
  type: string
- description: Human-readable description of the subscription
  name: description
  type: string
- description: ''
  name: retryPolicy
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-subscription-schema.json
slug: argus-enterprise-subscription
source_filename: argus-enterprise-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-subscription-schema.json\",\n  \"title\": \"Subscription\",\n  \"description\": \"Subscription schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique subscription identifier\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS endpoint URL for webhook delivery\"\n    },\n    \"eventTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"property.created\",\n          \"property.updated\",\n          \"property.deleted\",\n          \"valuation.created\",\n          \"valuation.updated\",\n          \"lease.created\",\n       \
  \   \"lease.updated\",\n          \"lease.expired\",\n          \"portfolio.created\",\n          \"portfolio.updated\",\n          \"portfolio.deleted\",\n          \"report.completed\",\n          \"report.failed\",\n          \"cashflow.updated\",\n          \"tenant.created\",\n          \"tenant.updated\"\n        ]\n      },\n      \"description\": \"Event types this subscription receives\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Paused\",\n        \"Disabled\"\n      ],\n      \"description\": \"Current subscription status\"\n    },\n    \"secret\": {\n      \"type\": \"string\",\n      \"description\": \"Shared secret for HMAC-SHA256 signature verification of webhook payloads (only returned on creation)\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the subscription\"\n    },\n    \"retryPolicy\": {\n      \"$ref\": \"#/components/schemas/RetryPolicy\"\
  \n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-subscription-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Subscription
---
