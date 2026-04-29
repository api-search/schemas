---
description: Authentication credentials for API sign-in.
layout: schema
name: SignAppInRequest
properties_list:
- description: The Application ID registered in BeyondTrust.
  name: ApplicationID
  type: string
- description: The API key for the application.
  name: APIKey
  type: string
provider_name: BeyondTrust
provider_slug: beyondtrust
schema_file: json-schema/beyondtrust-sign-app-in-request-schema.json
slug: beyondtrust-sign-app-in-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-sign-app-in-request-schema.json\",\n  \"title\": \"SignAppInRequest\",\n  \"description\": \"Authentication credentials for API sign-in.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationID\": {\n      \"type\": \"string\",\n      \"description\": \"The Application ID registered in BeyondTrust.\",\n      \"example\": \"myapp-api\"\n    },\n    \"APIKey\": {\n      \"type\": \"string\",\n      \"description\": \"The API key for the application.\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    }\n  },\n  \"required\": [\n    \"ApplicationID\",\n    \"APIKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/beyondtrust/refs/heads/main/json-schema/beyondtrust-sign-app-in-request-schema.json
tags:
- Access
- Access Management
- Compliance
- Credentials
- Privileged Access
- Security
- Secrets
- Zero Trust
title: SignAppInRequest
---
