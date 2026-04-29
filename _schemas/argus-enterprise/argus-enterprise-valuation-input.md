---
description: ValuationInput schema from ARGUS Enterprise API
layout: schema
name: ValuationInput
properties_list:
- description: ''
  name: valuationDate
  type: string
- description: ''
  name: methodology
  type: string
- description: ''
  name: marketValue
  type: number
- description: ''
  name: capRate
  type: number
- description: ''
  name: discountRate
  type: number
- description: ''
  name: terminalCapRate
  type: number
- description: ''
  name: analysisStartDate
  type: string
- description: ''
  name: analysisEndDate
  type: string
- description: ''
  name: netOperatingIncome
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: notes
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-valuation-input-schema.json
slug: argus-enterprise-valuation-input
source_filename: argus-enterprise-valuation-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-valuation-input-schema.json\",\n  \"title\": \"ValuationInput\",\n  \"description\": \"ValuationInput schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"valuationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"methodology\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DCF\",\n        \"DirectCapitalization\",\n        \"ComparableSales\"\n      ]\n    },\n    \"marketValue\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"capRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"discountRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"terminalCapRate\": {\n      \"type\": \"number\",\n      \"format\": \"\
  double\"\n    },\n    \"analysisStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"analysisEndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"netOperatingIncome\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\"\n    },\n    \"notes\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"valuationDate\",\n    \"methodology\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-valuation-input-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: ValuationInput
---
