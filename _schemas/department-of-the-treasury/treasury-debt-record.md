---
description: A single daily observation from the Debt to the Penny dataset.
layout: schema
name: Debt to the Penny Record
properties_list:
- description: ''
  name: record_date
  type: string
- description: Debt held by the public, in U.S. dollars (string-encoded decimal).
  name: debt_held_public_amt
  type: string
- description: Intragovernmental holdings, in U.S. dollars.
  name: intragov_hold_amt
  type: string
- description: Total public debt outstanding, in U.S. dollars.
  name: tot_pub_debt_out_amt
  type: string
- description: ''
  name: src_line_nbr
  type:
  - string
  - integer
- description: ''
  name: record_fiscal_year
  type: string
- description: ''
  name: record_fiscal_quarter
  type: string
- description: ''
  name: record_calendar_year
  type: string
- description: ''
  name: record_calendar_quarter
  type: string
- description: ''
  name: record_calendar_month
  type: string
- description: ''
  name: record_calendar_day
  type: string
provider_name: Department of the Treasury
provider_slug: department-of-the-treasury
schema_file: json-schema/treasury-debt-record-schema.json
slug: treasury-debt-record
source_filename: treasury-debt-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-the-treasury/schemas/debt-to-the-penny.json\",\n  \"title\": \"Debt to the Penny Record\",\n  \"description\": \"A single daily observation from the Debt to the Penny dataset.\",\n  \"type\": \"object\",\n  \"required\": [\"record_date\", \"tot_pub_debt_out_amt\"],\n  \"properties\": {\n    \"record_date\": { \"type\": \"string\", \"format\": \"date\" },\n    \"debt_held_public_amt\": { \"type\": \"string\", \"description\": \"Debt held by the public, in U.S. dollars (string-encoded decimal).\" },\n    \"intragov_hold_amt\": { \"type\": \"string\", \"description\": \"Intragovernmental holdings, in U.S. dollars.\" },\n    \"tot_pub_debt_out_amt\": { \"type\": \"string\", \"description\": \"Total public debt outstanding, in U.S. dollars.\" },\n    \"src_line_nbr\": { \"type\": [\"string\", \"integer\"] },\n    \"record_fiscal_year\": { \"type\": \"string\"\
  , \"pattern\": \"^[0-9]{4}$\" },\n    \"record_fiscal_quarter\": { \"type\": \"string\" },\n    \"record_calendar_year\": { \"type\": \"string\", \"pattern\": \"^[0-9]{4}$\" },\n    \"record_calendar_quarter\": { \"type\": \"string\" },\n    \"record_calendar_month\": { \"type\": \"string\" },\n    \"record_calendar_day\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-treasury/refs/heads/main/json-schema/treasury-debt-record-schema.json
tags:
- Federal Government
- Finance
- Debt
- Sanctions
title: Debt to the Penny Record
---
