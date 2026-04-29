---
description: LeaseOption schema from ARGUS Enterprise API
layout: schema
name: LeaseOption
properties_list:
- description: Type of lease option
  name: optionType
  type: string
- description: Date by which notice must be given
  name: noticeDate
  type: string
- description: Date the option can be exercised
  name: exerciseDate
  type: string
- description: Duration of option term in months
  name: termMonths
  type: integer
- description: Description of rent adjustment terms
  name: rentAdjustment
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-lease-option-schema.json
slug: argus-enterprise-lease-option
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-lease-option-schema.json\",\n  \"title\": \"LeaseOption\",\n  \"description\": \"LeaseOption schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"optionType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Renewal\",\n        \"Expansion\",\n        \"Termination\",\n        \"PurchaseOption\"\n      ],\n      \"description\": \"Type of lease option\"\n    },\n    \"noticeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date by which notice must be given\"\n    },\n    \"exerciseDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the option can be exercised\"\n    },\n    \"termMonths\": {\n      \"type\": \"integer\",\n      \"description\": \"\
  Duration of option term in months\"\n    },\n    \"rentAdjustment\": {\n      \"type\": \"string\",\n      \"description\": \"Description of rent adjustment terms\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-lease-option-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: LeaseOption
---
