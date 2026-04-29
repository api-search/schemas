---
description: Represents a single sign-in attempt to a 1Password account.
layout: schema
name: SignInAttempt
properties_list:
- description: The unique identifier for the sign-in attempt.
  name: uuid
  type: string
- description: The UUID of the session associated with the sign-in attempt.
  name: session_uuid
  type: string
- description: When the sign-in attempt occurred.
  name: timestamp
  type: string
- description: The category of the sign-in attempt.
  name: category
  type: string
- description: The type of sign-in method used.
  name: type
  type: string
- description: The two-letter ISO country code of the sign-in location.
  name: country
  type: string
- description: ''
  name: target_user
  type: object
- description: ''
  name: client
  type: object
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-events-sign-in-attempt-schema.json
slug: 1password-events-sign-in-attempt
source_filename: 1password-events-sign-in-attempt-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-sign-in-attempt-schema.json\",\n  \"title\": \"SignInAttempt\",\n  \"description\": \"Represents a single sign-in attempt to a 1Password account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the sign-in attempt.\"\n    },\n    \"session_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the session associated with the sign-in attempt.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the sign-in attempt occurred.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the sign-in attempt.\"\
  ,\n      \"enum\": [\n        \"success\",\n        \"credentials_failed\",\n        \"mfa_failed\",\n        \"modern_version_required\",\n        \"sso_failed\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of sign-in method used.\",\n      \"enum\": [\n        \"credentials_ok\",\n        \"mfa_ok\",\n        \"password_secret_bad\",\n        \"mfa_missing\",\n        \"totp_disabled\",\n        \"totp_bad\",\n        \"u2f_failed\",\n        \"duo_failed\",\n        \"duo_native_failed\",\n        \"sso_failed\"\n      ]\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The two-letter ISO country code of the sign-in location.\",\n      \"minLength\": 2,\n      \"maxLength\": 2\n    },\n    \"target_user\": {\n      \"$ref\": \"#/components/schemas/EventUser\"\n    },\n    \"client\": {\n      \"$ref\": \"#/components/schemas/EventClient\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-events-sign-in-attempt-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: SignInAttempt
---
