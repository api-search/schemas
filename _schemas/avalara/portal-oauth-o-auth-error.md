---
description: OAuthError schema from Avalara API
layout: schema
name: OAuthError
properties_list:
- description: ''
  name: error
  type: string
- description: ''
  name: error_description
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/portal-oauth-o-auth-error-schema.json
slug: portal-oauth-o-auth-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/portal-oauth-o-auth-error-schema.json\",\n  \"title\": \"OAuthError\",\n  \"description\": \"OAuthError schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"invalid_request\",\n        \"invalid_client\",\n        \"invalid_grant\",\n        \"unauthorized_client\",\n        \"unsupported_grant_type\",\n        \"invalid_scope\"\n      ]\n    },\n    \"error_description\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/portal-oauth-o-auth-error-schema.json
tags:
- Taxes
title: OAuthError
---
