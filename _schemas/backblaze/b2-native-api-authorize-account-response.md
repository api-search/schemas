---
description: Response from the b2_authorize_account operation
layout: schema
name: AuthorizeAccountResponse
properties_list:
- description: The identifier for the account
  name: accountId
  type: string
- description: An authorization token to use with all calls other than b2_authorize_account
  name: authorizationToken
  type: string
- description: ''
  name: allowed
  type: object
- description: ''
  name: apiInfo
  type: object
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-authorize-account-response-schema.json
slug: b2-native-api-authorize-account-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-authorize-account-response-schema.json\",\n  \"title\": \"AuthorizeAccountResponse\",\n  \"description\": \"Response from the b2_authorize_account operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the account\",\n      \"example\": \"abc123def456\"\n    },\n    \"authorizationToken\": {\n      \"type\": \"string\",\n      \"description\": \"An authorization token to use with all calls other than b2_authorize_account\",\n      \"example\": \"4_002acd2a08df7f8c0c4d21e9deef28c7\"\n    },\n    \"allowed\": {\n      \"$ref\": \"#/components/schemas/AllowedCapabilities\"\n    },\n    \"apiInfo\": {\n      \"$ref\": \"#/components/schemas/ApiInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-authorize-account-response-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: AuthorizeAccountResponse
---
