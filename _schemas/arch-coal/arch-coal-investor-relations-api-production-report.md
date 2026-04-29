---
description: ''
layout: schema
name: ProductionReport
properties_list:
- description: Fiscal year
  name: year
  type: integer
- description: Quarter
  name: quarter
  type: integer
- description: Total coal production in short tons
  name: totalTons
  type: integer
- description: Metallurgical coal production in short tons
  name: metCoalTons
  type: integer
- description: Thermal coal production in short tons
  name: thermalCoalTons
  type: integer
- description: Average realized price per short ton in USD
  name: averagePrice
  type: number
provider_name: Arch Coal
provider_slug: arch-coal
schema_file: json-schema/arch-coal-investor-relations-api-production-report-schema.json
slug: arch-coal-investor-relations-api-production-report
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"year\": {\n      \"type\": \"integer\",\n      \"description\": \"Fiscal year\",\n      \"example\": 2025\n    },\n    \"quarter\": {\n      \"type\": \"integer\",\n      \"description\": \"Quarter\",\n      \"example\": 4\n    },\n    \"totalTons\": {\n      \"type\": \"integer\",\n      \"description\": \"Total coal production in short tons\",\n      \"example\": 5800000\n    },\n    \"metCoalTons\": {\n      \"type\": \"integer\",\n      \"description\": \"Metallurgical coal production in short tons\",\n      \"example\": 4100000\n    },\n    \"thermalCoalTons\": {\n      \"type\": \"integer\",\n      \"description\": \"Thermal coal production in short tons\",\n      \"example\": 1700000\n    },\n    \"averagePrice\": {\n      \"type\": \"number\",\n      \"description\": \"Average realized price per short ton in USD\",\n      \"example\": 172.5\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/json-schema/arch-coal-investor-relations-api-production-report-schema.json\",\n  \"title\": \"ProductionReport\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arch-coal/refs/heads/main/json-schema/arch-coal-investor-relations-api-production-report-schema.json
tags:
- Mining
- Coal
- Metallurgical Coal
- Thermal Coal
- Energy
- Fortune 500
title: ProductionReport
---
