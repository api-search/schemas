---
description: UsernameType schema from Amazon Cognito
layout: schema
name: UsernameType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-username-type-schema.json
slug: cognito-idp-username-type
source_filename: cognito-idp-username-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"[\\\\p{L}\\\\p{M}\\\\p{S}\\\\p{N}\\\\p{P}]+\",\n  \"minLength\": 1,\n  \"maxLength\": 128,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-username-type-schema.json\",\n  \"title\": \"UsernameType\",\n  \"description\": \"UsernameType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-username-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UsernameType
---
