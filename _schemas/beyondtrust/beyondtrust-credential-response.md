---
description: Credentials retrieved for an approved access request.
layout: schema
name: CredentialResponse
properties_list:
- description: The retrieved password. Only present for password-based accounts.
  name: Password
  type: string
- description: SSH private key. Only present for SSH key-based accounts.
  name: PrivateKey
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-credential-response-schema.json
slug: beyondtrust-credential-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-credential-response-schema.json\",\n  \"title\": \"CredentialResponse\",\n  \"description\": \"Credentials retrieved for an approved access request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Password\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"The retrieved password. Only present for password-based accounts.\",\n      \"example\": \"Xk2!mP9@nQ7#rT5\"\n    },\n    \"PrivateKey\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"SSH private key. Only present for SSH key-based accounts.\",\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-credential-response-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: CredentialResponse
---
