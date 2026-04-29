---
description: Request to create an access credential.
layout: schema
name: CredentialInput
properties_list:
- description: ID of the user.
  name: userId
  type: string
- description: Credential type.
  name: type
  type: string
- description: Card number for badge credentials.
  name: cardNumber
  type: string
provider_name: ADT
provider_slug: adt
schema_file: json-schema/business-api-credential-input-schema.json
slug: business-api-credential-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-credential-input-schema.json\",\n  \"title\": \"CredentialInput\",\n  \"description\": \"Request to create an access credential.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"userId\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user.\",\n      \"example\": \"usr-001\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Credential type.\",\n      \"enum\": [\n        \"badge\",\n        \"pin\",\n        \"mobile\"\n      ]\n    },\n    \"cardNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Card number for badge credentials.\",\n      \"example\": \"1234567890\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-credential-input-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: CredentialInput
---
