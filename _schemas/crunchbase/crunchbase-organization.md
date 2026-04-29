---
description: Schema for a Crunchbase organization (company, investor, or school) entity.
layout: schema
name: CrunchbaseOrganization
properties_list:
- description: ''
  name: uuid
  type: string
- description: ''
  name: permalink
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: short_description
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: website_url
  type: string
- description: ''
  name: linkedin
  type: string
- description: ''
  name: twitter
  type: string
- description: ''
  name: founded_on
  type: string
- description: ''
  name: closed_on
  type: string
- description: ''
  name: operating_status
  type: string
- description: ''
  name: num_employees_enum
  type: string
- description: ''
  name: ipo_status
  type: string
- description: ''
  name: category_groups
  type: array
- description: ''
  name: categories
  type: array
- description: ''
  name: location_identifiers
  type: array
- description: ''
  name: funding_total
  type: object
- description: ''
  name: last_funding_at
  type: string
- description: ''
  name: last_funding_type
  type: string
- description: ''
  name: num_funding_rounds
  type: integer
- description: ''
  name: num_investors
  type: integer
- description: ''
  name: num_acquisitions
  type: integer
- description: ''
  name: num_investments
  type: integer
provider_name: Crunchbase
provider_slug: crunchbase
schema_file: json-schema/crunchbase-organization-schema.json
slug: crunchbase-organization
source_filename: crunchbase-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crunchbase/refs/heads/main/json-schema/crunchbase-organization-schema.json\",\n  \"title\": \"CrunchbaseOrganization\",\n  \"description\": \"Schema for a Crunchbase organization (company, investor, or school) entity.\",\n  \"type\": \"object\",\n  \"required\": [\"uuid\", \"name\"],\n  \"properties\": {\n    \"uuid\": {\"type\": \"string\", \"format\": \"uuid\"},\n    \"permalink\": {\"type\": \"string\"},\n    \"name\": {\"type\": \"string\"},\n    \"short_description\": {\"type\": \"string\"},\n    \"description\": {\"type\": \"string\"},\n    \"website_url\": {\"type\": \"string\", \"format\": \"uri\"},\n    \"linkedin\": {\"type\": \"string\", \"format\": \"uri\"},\n    \"twitter\": {\"type\": \"string\", \"format\": \"uri\"},\n    \"founded_on\": {\"type\": \"string\", \"format\": \"date\"},\n    \"closed_on\": {\"type\": \"string\", \"format\"\
  : \"date\"},\n    \"operating_status\": {\"type\": \"string\", \"enum\": [\"active\", \"closed\"]},\n    \"num_employees_enum\": {\"type\": \"string\"},\n    \"ipo_status\": {\"type\": \"string\", \"enum\": [\"private\", \"public\", \"delisted\", \"was_acquired\"]},\n    \"category_groups\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\"}\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\"type\": \"string\"}\n    },\n    \"location_identifiers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"uuid\": {\"type\": \"string\", \"format\": \"uuid\"},\n          \"value\": {\"type\": \"string\"},\n          \"permalink\": {\"type\": \"string\"}\n        }\n      }\n    },\n    \"funding_total\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\"type\": \"number\"},\n        \"currency\": {\"type\": \"string\"},\n        \"value_usd\": {\"\
  type\": \"number\"}\n      }\n    },\n    \"last_funding_at\": {\"type\": \"string\", \"format\": \"date\"},\n    \"last_funding_type\": {\"type\": \"string\"},\n    \"num_funding_rounds\": {\"type\": \"integer\"},\n    \"num_investors\": {\"type\": \"integer\"},\n    \"num_acquisitions\": {\"type\": \"integer\"},\n    \"num_investments\": {\"type\": \"integer\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crunchbase/refs/heads/main/json-schema/crunchbase-organization-schema.json
tags:
- Business Data
- Funding
- Investments
- Startups
- Private Markets
- Firmographics
title: CrunchbaseOrganization
---
