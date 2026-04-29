---
description: Represents a record of an API request made to the Connect server.
layout: schema
name: APIRequest
properties_list:
- description: The unique identifier for the API request.
  name: requestId
  type: string
- description: When the request was made.
  name: timestamp
  type: string
- description: The HTTP method of the request.
  name: action
  type: string
- description: The result status of the request.
  name: result
  type: string
- description: The actor who made the request.
  name: actor
  type: object
- description: The resource that was accessed.
  name: resource
  type: object
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-api-request-schema.json
slug: 1password-connect-api-request
source_filename: 1password-connect-api-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-api-request-schema.json\",\n  \"title\": \"APIRequest\",\n  \"description\": \"Represents a record of an API request made to the Connect server.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the API request.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the request was made.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP method of the request.\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"description\": \"The result status of the request.\",\n      \"enum\": [\n        \"SUCCESS\",\n        \"DENY\"\n      ]\n   \
  \ },\n    \"actor\": {\n      \"type\": \"object\",\n      \"description\": \"The actor who made the request.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the actor.\"\n        },\n        \"account\": {\n          \"type\": \"string\",\n          \"description\": \"The account associated with the actor.\"\n        },\n        \"jti\": {\n          \"type\": \"string\",\n          \"description\": \"The JWT token identifier.\"\n        },\n        \"userAgent\": {\n          \"type\": \"string\",\n          \"description\": \"The user agent string of the client.\"\n        },\n        \"requestIp\": {\n          \"type\": \"string\",\n          \"description\": \"The IP address of the client.\"\n        }\n      }\n    },\n    \"resource\": {\n      \"type\": \"object\",\n      \"description\": \"The resource that was accessed.\",\n      \"properties\": {\n       \
  \ \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of resource.\"\n        },\n        \"vault\": {\n          \"$ref\": \"#/components/schemas/VaultRef\"\n        },\n        \"item\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\",\n              \"description\": \"The unique identifier of the item.\"\n            }\n          }\n        },\n        \"itemVersion\": {\n          \"type\": \"integer\",\n          \"description\": \"The version of the item.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-api-request-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: APIRequest
---
