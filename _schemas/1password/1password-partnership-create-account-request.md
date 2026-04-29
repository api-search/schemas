---
description: The request body for creating a new partner billing account.
layout: schema
name: CreateAccountRequest
properties_list:
- description: The unique identifier for the customer's billing account, supplied by the partner. Can be up to 200 characters with alphanumeric characters, hyphens, and periods.
  name: account_uid
  type: string
- description: The 1Password account type for the customer. Individual (I) or Family (F). Team and business accounts are not supported.
  name: account_type
  type: string
- description: The domain the customer can use for their new or existing 1Password account.
  name: domain
  type: string
- description: The optional date and time to remove the customer's account from the partner billing service. ISO 8601 format.
  name: ends_at
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-partnership-create-account-request-schema.json
slug: 1password-partnership-create-account-request
source_filename: 1password-partnership-create-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-partnership-create-account-request-schema.json\",\n  \"title\": \"CreateAccountRequest\",\n  \"description\": \"The request body for creating a new partner billing account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account_uid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the customer's billing account, supplied by the partner. Can be up to 200 characters with alphanumeric characters, hyphens, and periods.\",\n      \"maxLength\": 200,\n      \"pattern\": \"^[A-Za-z0-9.\\\\-]+$\"\n    },\n    \"account_type\": {\n      \"type\": \"string\",\n      \"description\": \"The 1Password account type for the customer. Individual (I) or Family (F). Team and business accounts are not supported.\",\n      \"enum\": [\n        \"I\",\n        \"F\"\n      ]\n\
  \    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain the customer can use for their new or existing 1Password account.\"\n    },\n    \"ends_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The optional date and time to remove the customer's account from the partner billing service. ISO 8601 format.\"\n    }\n  },\n  \"required\": [\n    \"account_uid\",\n    \"account_type\",\n    \"domain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-partnership-create-account-request-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: CreateAccountRequest
---
