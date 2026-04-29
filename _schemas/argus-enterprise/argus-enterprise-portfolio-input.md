---
description: PortfolioInput schema from ARGUS Enterprise API
layout: schema
name: PortfolioInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: strategy
  type: string
- description: ''
  name: currency
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-portfolio-input-schema.json
slug: argus-enterprise-portfolio-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-portfolio-input-schema.json\",\n  \"title\": \"PortfolioInput\",\n  \"description\": \"PortfolioInput schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Core\",\n        \"CorePlus\",\n        \"ValueAdd\",\n        \"Opportunistic\"\n      ]\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-portfolio-input-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: PortfolioInput
---
