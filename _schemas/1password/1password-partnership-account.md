---
description: Represents a partner billing account for a 1Password customer.
layout: schema
name: Account
properties_list:
- description: The unique identifier for the customer's billing account.
  name: account_uid
  type: string
- description: The 1Password account type. I for individual, F for family.
  name: account_type
  type: string
- description: The domain associated with the customer's 1Password account.
  name: domain
  type: string
- description: The current status of the partner billing account.
  name: status
  type: string
- description: The unique activation token used to link the customer's 1Password account with their partner billing account. Append this to a 1Password partnership redemption link.
  name: activation_token
  type: string
- description: The date and time the customer's account is scheduled to be removed from the partner billing service.
  name: ends_at
  type: string
- description: The date and time the billing account was created.
  name: created_at
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-partnership-account-schema.json
slug: 1password-partnership-account
source_filename: 1password-partnership-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-partnership-account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"Represents a partner billing account for a 1Password customer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account_uid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the customer's billing account.\"\n    },\n    \"account_type\": {\n      \"type\": \"string\",\n      \"description\": \"The 1Password account type. I for individual, F for family.\",\n      \"enum\": [\n        \"I\",\n        \"F\"\n      ]\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain associated with the customer's 1Password account.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the partner billing\
  \ account.\",\n      \"enum\": [\n        \"entitled\",\n        \"provisioned\",\n        \"activated\",\n        \"suspended\",\n        \"deprovisioned\"\n      ]\n    },\n    \"activation_token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique activation token used to link the customer's 1Password account with their partner billing account. Append this to a 1Password partnership redemption link.\"\n    },\n    \"ends_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the customer's account is scheduled to be removed from the partner billing service.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the billing account was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-partnership-account-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: Account
---
