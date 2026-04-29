---
description: Specify which fields to update in `updateMask` and provide corresponding values in `connection`. Fields in `connection` not listed in `updateMask` are ignored.
layout: schema
name: UpdateConnectionRequest
properties_list:
- description: Fields to update. Each entry must have a corresponding value in `connection`. Credential fields (`apiKey`, `basicAuth`, `oauth2ClientCredentials`, `oauth2PasswordCredentials`) must match the connectio
  name: updateMask
  type: array
- description: ''
  name: connection
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-update-connection-request-schema.json
slug: ampersand-api-update-connection-request
source_filename: ampersand-api-update-connection-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-update-connection-request-schema.json\",\n  \"title\": \"UpdateConnectionRequest\",\n  \"description\": \"Specify which fields to update in `updateMask` and provide corresponding values in `connection`. Fields in `connection` not listed in `updateMask` are ignored.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateMask\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"providerWorkspaceRef\",\n          \"providerMetadata\",\n          \"apiKey\",\n          \"basicAuth\",\n          \"oauth2ClientCredentials\",\n          \"oauth2PasswordCredentials\"\n        ]\n      },\n      \"description\": \"Fields to update. Each entry must have a corresponding value in `connection`. Credential fields (`apiKey`, `basicAuth`,\
  \ `oauth2ClientCredentials`, `oauth2PasswordCredentials`) must match the connection's existing auth scheme.\",\n      \"example\": [\n        \"apiKey\"\n      ]\n    },\n    \"connection\": {\n      \"$ref\": \"#/components/schemas/ConnectionRequest\"\n    }\n  },\n  \"required\": [\n    \"updateMask\",\n    \"connection\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-update-connection-request-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: UpdateConnectionRequest
---
