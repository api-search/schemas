---
description: Set of Personally Identifiable Information (PII) associated with a given client.
layout: schema
name: Profile
properties_list:
- description: Maiden name of the client. <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: maidenName
  type: string
- description: 'Date of birth. <br/> **Conditional Mandatory**<font color=''red''>* </font> field - Required while creating new client. <br/> Date format must be ISO 8601: `YYYY-MM-DD` <br/> where: <br/> YYYY = four-di'
  name: birthDate
  type: string
- description: Birth city of the client. City will be verified against the 'city master setup'. <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: birthCity
  type: string
- description: Expressed as a 2-letter (Alpha-2) country code as defined in ISO 3166. <br/> For example - IN, US, CA, GB <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font
  name: birthCountry
  type: string
- description: The status of belonging to a particular nation. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client. <br/> Expressed as a 2-letter (Alpha-2) country c
  name: nationality
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-profile-schema.json
slug: mastercard-card-issuance-profile
source_filename: mastercard-card-issuance-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Profile\",\n  \"type\": \"object\",\n  \"description\": \"Set of Personally Identifiable Information (PII) associated with a given client.\",\n  \"properties\": {\n    \"maidenName\": {\n      \"type\": \"string\",\n      \"description\": \"Maiden name of the client. <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of birth. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client. <br/> Date format must be ISO 8601: `YYYY-MM-DD`  <br/> where:  <br/> YYYY = four-digit year  <br/> MM   = two-digit month (01=January, etc.)  <br/> DD = two-digit day of month (01 through 31, as applicable)\"\n    },\n    \"birthCity\": {\n      \"type\": \"string\",\n      \"description\": \"Birth city of the client. City will be\
  \ verified against the 'city master setup'. <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"birthCountry\": {\n      \"type\": \"string\",\n      \"description\": \"Expressed as a 2-letter (Alpha-2) country code as defined in ISO 3166. <br/> For example - IN, US, CA, GB <br/> This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"nationality\": {\n      \"type\": \"string\",\n      \"description\": \"The status of belonging to a particular nation. <br/> **Conditional Mandatory**<font color='red'>* </font> field - Required while creating new client. <br/> Expressed as a 2-letter (Alpha-2) country code as defined in ISO 3166. <br/> For example - IN, US, CA, GB\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-profile-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Profile
---
