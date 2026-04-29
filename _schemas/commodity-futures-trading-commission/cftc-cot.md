---
description: Common base schema for a row of CFTC Commitments of Traders data returned by the SODA endpoints at publicreporting.cftc.gov. Specific report formats add additional category breakdowns.
layout: schema
name: CFTC Commitments of Traders Row
properties_list:
- description: Combined market and exchange name as published by the CFTC.
  name: market_and_exchange_names
  type: string
- description: Report Tuesday for the COT week.
  name: report_date_as_yyyy_mm_dd
  type: string
- description: CFTC contract market code identifying the underlying contract.
  name: cftc_contract_market_code
  type: string
- description: CFTC market code.
  name: cftc_market_code
  type: string
- description: CFTC region code.
  name: cftc_region_code
  type: string
- description: CFTC commodity code (DCOT).
  name: cftc_commodity_code
  type: string
- description: Total reportable plus non-reportable open interest in the contract.
  name: open_interest_all
  type: string
provider_name: Commodity Futures Trading Commission
provider_slug: commodity-futures-trading-commission
schema_file: json-schema/cftc-cot-schema.json
slug: cftc-cot
source_filename: cftc-cot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://publicreporting.cftc.gov/schemas/cot-row.json\",\n  \"title\": \"CFTC Commitments of Traders Row\",\n  \"description\": \"Common base schema for a row of CFTC Commitments of Traders data returned by the SODA endpoints at publicreporting.cftc.gov. Specific report formats add additional category breakdowns.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"market_and_exchange_names\": {\n      \"type\": \"string\",\n      \"description\": \"Combined market and exchange name as published by the CFTC.\"\n    },\n    \"report_date_as_yyyy_mm_dd\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Report Tuesday for the COT week.\"\n    },\n    \"cftc_contract_market_code\": {\n      \"type\": \"string\",\n      \"description\": \"CFTC contract market code identifying the underlying contract.\"\n    },\n    \"cftc_market_code\": {\n      \"type\": \"\
  string\",\n      \"description\": \"CFTC market code.\"\n    },\n    \"cftc_region_code\": {\n      \"type\": \"string\",\n      \"description\": \"CFTC region code.\"\n    },\n    \"cftc_commodity_code\": {\n      \"type\": \"string\",\n      \"description\": \"CFTC commodity code (DCOT).\"\n    },\n    \"open_interest_all\": {\n      \"type\": \"string\",\n      \"description\": \"Total reportable plus non-reportable open interest in the contract.\"\n    }\n  },\n  \"required\": [\n    \"market_and_exchange_names\",\n    \"report_date_as_yyyy_mm_dd\",\n    \"cftc_contract_market_code\",\n    \"open_interest_all\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/commodity-futures-trading-commission/refs/heads/main/json-schema/cftc-cot-schema.json
tags:
- CFTC
- Commitments of Traders
- Federal Government
- Financial
- Futures
- Open Data
- SODA
- Trading
title: CFTC Commitments of Traders Row
---
