---
description: IdentityId schema from Amazon Cognito
layout: schema
name: IdentityId
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-identity-id-schema.json
slug: cognito-identity-identity-id
source_filename: cognito-identity-identity-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"[\\\\w-]+:[0-9a-f-]+\",\n  \"minLength\": 1,\n  \"maxLength\": 55,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identity-id-schema.json\",\n  \"title\": \"IdentityId\",\n  \"description\": \"IdentityId schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identity-id-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: IdentityId
---
