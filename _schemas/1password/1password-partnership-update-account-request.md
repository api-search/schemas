---
description: The request body for updating a partner billing account.
layout: schema
name: UpdateAccountRequest
properties_list:
- description: The date and time to schedule removal of the customer's billing account from the partner billing service. ISO 8601 format.
  name: ends_at
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-partnership-update-account-request-schema.json
slug: 1password-partnership-update-account-request
source_filename: 1password-partnership-update-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-partnership-update-account-request-schema.json\",\n  \"title\": \"UpdateAccountRequest\",\n  \"description\": \"The request body for updating a partner billing account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ends_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time to schedule removal of the customer's billing account from the partner billing service. ISO 8601 format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-partnership-update-account-request-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: UpdateAccountRequest
---
