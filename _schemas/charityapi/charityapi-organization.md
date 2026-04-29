---
description: A US nonprofit organization record sourced from the IRS Business Master File.
layout: schema
name: CharityAPI Organization
properties_list:
- description: Employer Identification Number.
  name: ein
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: ico
  type: string
- description: ''
  name: street
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: zip
  type: string
- description: ''
  name: subsection
  type: string
- description: ''
  name: affiliation
  type: string
- description: ''
  name: classification
  type: string
- description: ''
  name: ruling
  type: string
- description: ''
  name: deductibility
  type: string
- description: ''
  name: foundation
  type: string
- description: ''
  name: activity
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: tax_period
  type: string
- description: ''
  name: asset_amt
  type: integer
- description: ''
  name: income_amt
  type: integer
- description: ''
  name: revenue_amt
  type: integer
- description: ''
  name: ntee_cd
  type: string
provider_name: CharityAPI
provider_slug: charityapi
schema_file: json-schema/charityapi-organization-schema.json
slug: charityapi-organization
source_filename: charityapi-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://charityapi.org/schemas/organization.json\",\n  \"title\": \"CharityAPI Organization\",\n  \"description\": \"A US nonprofit organization record sourced from the IRS Business Master File.\",\n  \"type\": \"object\",\n  \"required\": [\"ein\", \"name\"],\n  \"properties\": {\n    \"ein\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9]{9}$\",\n      \"description\": \"Employer Identification Number.\"\n    },\n    \"name\": { \"type\": \"string\" },\n    \"ico\": { \"type\": \"string\" },\n    \"street\": { \"type\": \"string\" },\n    \"city\": { \"type\": \"string\" },\n    \"state\": { \"type\": \"string\" },\n    \"zip\": { \"type\": \"string\" },\n    \"subsection\": { \"type\": \"string\" },\n    \"affiliation\": { \"type\": \"string\" },\n    \"classification\": { \"type\": \"string\" },\n    \"ruling\": { \"type\": \"string\" },\n    \"deductibility\": { \"type\": \"\
  string\" },\n    \"foundation\": { \"type\": \"string\" },\n    \"activity\": { \"type\": \"string\" },\n    \"status\": { \"type\": \"string\" },\n    \"tax_period\": { \"type\": \"string\" },\n    \"asset_amt\": { \"type\": \"integer\" },\n    \"income_amt\": { \"type\": \"integer\" },\n    \"revenue_amt\": { \"type\": \"integer\" },\n    \"ntee_cd\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charityapi/refs/heads/main/json-schema/charityapi-organization-schema.json
tags:
- 501c3
- Charities
- Donations
- EIN
- IRS
- Non-Profits
- Tax Compliance
- Verification
title: CharityAPI Organization
---
