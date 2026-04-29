---
description: SubscriptionList schema from ARGUS Enterprise API
layout: schema
name: SubscriptionList
properties_list:
- description: ''
  name: data
  type: array
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-subscription-list-schema.json
slug: argus-enterprise-subscription-list
source_filename: argus-enterprise-subscription-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-subscription-list-schema.json\",\n  \"title\": \"SubscriptionList\",\n  \"description\": \"SubscriptionList schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Subscription\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-subscription-list-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: SubscriptionList
---
