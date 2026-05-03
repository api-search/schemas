---
description: An Account in Salesloft represents a company or organization being tracked in the sales process.
layout: schema
name: Salesloft Account
properties_list:
- description: Unique identifier for the account
  name: id
  type: integer
- description: The full name of the account
  name: name
  type: string
- description: The web domain of the account
  name: domain
  type: string
- description: Short conversational name for the account
  name: conversational_name
  type: string
- description: Free-text description of the account
  name: description
  type: string
- description: Primary phone number of the account
  name: phone
  type: string
- description: Company website URL
  name: website
  type: string
- description: LinkedIn profile URL of the company
  name: linkedin_url
  type: string
- description: Twitter handle of the company
  name: twitter_handle
  type: string
- description: Street address
  name: street
  type: string
- description: City
  name: city
  type: string
- description: State or province
  name: state
  type: string
- description: Postal/ZIP code
  name: postal_code
  type: string
- description: Country
  name: country
  type: string
- description: Locale for the account (e.g. en_US)
  name: locale
  type: string
- description: Industry vertical
  name: industry
  type: string
- description: Type of company (e.g. private, public)
  name: company_type
  type: string
- description: Year the company was founded
  name: founded
  type: string
- description: Annual revenue range
  name: revenue_range
  type: string
- description: Company size by employee count range
  name: size
  type: string
- description: Whether this account is flagged as do not contact
  name: do_not_contact
  type: boolean
- description: Key-value pairs of custom field data
  name: custom_fields
  type: object
- description: Array of tags associated with the account
  name: tags
  type: array
- description: ID of the user who owns this account
  name: owner_id
  type: integer
- description: ID of the company stage
  name: company_stage_id
  type: integer
- description: ID of the account tier
  name: account_tier_id
  type: integer
- description: External CRM identifier
  name: crm_id
  type: string
- description: Type of external CRM (e.g. salesforce)
  name: crm_id_type
  type: string
- description: Timestamp when the account was created
  name: created_at
  type: string
- description: Timestamp when the account was last updated
  name: updated_at
  type: string
provider_name: Salesloft
provider_slug: salesloft
schema_file: json-schema/salesloft-account-schema.json
slug: salesloft-account
source_filename: salesloft-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/salesloft/json-schema/salesloft-account-schema.json\",\n  \"title\": \"Salesloft Account\",\n  \"description\": \"An Account in Salesloft represents a company or organization being tracked in the sales process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the account\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the account\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The web domain of the account\"\n    },\n    \"conversational_name\": {\n      \"type\": \"string\",\n      \"description\": \"Short conversational name for the account\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text description of the account\"\n    },\n    \"\
  phone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number of the account\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Company website URL\"\n    },\n    \"linkedin_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"LinkedIn profile URL of the company\"\n    },\n    \"twitter_handle\": {\n      \"type\": \"string\",\n      \"description\": \"Twitter handle of the company\"\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"description\": \"Street address\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province\"\n    },\n    \"postal_code\": {\n      \"type\": \"string\",\n      \"description\": \"Postal/ZIP code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country\"\n\
  \    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"Locale for the account (e.g. en_US)\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry vertical\"\n    },\n    \"company_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of company (e.g. private, public)\"\n    },\n    \"founded\": {\n      \"type\": \"string\",\n      \"description\": \"Year the company was founded\"\n    },\n    \"revenue_range\": {\n      \"type\": \"string\",\n      \"description\": \"Annual revenue range\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"Company size by employee count range\"\n    },\n    \"do_not_contact\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this account is flagged as do not contact\"\n    },\n    \"custom_fields\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs of custom field data\",\n      \"additionalProperties\"\
  : true\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Array of tags associated with the account\"\n    },\n    \"owner_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the user who owns this account\"\n    },\n    \"company_stage_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the company stage\"\n    },\n    \"account_tier_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the account tier\"\n    },\n    \"crm_id\": {\n      \"type\": \"string\",\n      \"description\": \"External CRM identifier\"\n    },\n    \"crm_id_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of external CRM (e.g. salesforce)\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the account was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the account was last updated\"\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesloft/refs/heads/main/json-schema/salesloft-account-schema.json
tags:
- Sales
- CRM
- Revenue
- Automation
- AI
title: Salesloft Account
---
