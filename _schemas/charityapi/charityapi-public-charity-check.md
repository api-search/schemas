---
description: Result returned by the public_charity_check endpoint indicating whether an EIN is a 501c3.
layout: schema
name: CharityAPI Public Charity Check
properties_list:
- description: ''
  name: ein
  type: string
- description: ''
  name: public_charity
  type: boolean
provider_name: CharityAPI
provider_slug: charityapi
schema_file: json-schema/charityapi-public-charity-check-schema.json
slug: charityapi-public-charity-check
source_filename: charityapi-public-charity-check-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://charityapi.org/schemas/public-charity-check.json\",\n  \"title\": \"CharityAPI Public Charity Check\",\n  \"description\": \"Result returned by the public_charity_check endpoint indicating whether an EIN is a 501c3.\",\n  \"type\": \"object\",\n  \"required\": [\"ein\", \"public_charity\"],\n  \"properties\": {\n    \"ein\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9]{9}$\"\n    },\n    \"public_charity\": {\n      \"type\": \"boolean\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charityapi/refs/heads/main/json-schema/charityapi-public-charity-check-schema.json
tags:
- 501c3
- Charities
- Donations
- EIN
- IRS
- Non-Profits
- Tax Compliance
- Verification
title: CharityAPI Public Charity Check
---
