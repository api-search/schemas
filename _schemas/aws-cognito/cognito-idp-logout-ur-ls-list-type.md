---
description: LogoutURLsListType schema from Amazon Cognito
layout: schema
name: LogoutURLsListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-logout-ur-ls-list-type-schema.json
slug: cognito-idp-logout-ur-ls-list-type
source_filename: cognito-idp-logout-ur-ls-list-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[\\\\p{L}\\\\p{M}\\\\p{S}\\\\p{N}\\\\p{P}]+\",\n    \"minLength\": 1,\n    \"maxLength\": 1024\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-logout-ur-ls-list-type-schema.json\",\n  \"title\": \"LogoutURLsListType\",\n  \"description\": \"LogoutURLsListType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-logout-ur-ls-list-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: LogoutURLsListType
---
