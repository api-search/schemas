---
description: ClaimName schema from Amazon Cognito
layout: schema
name: ClaimName
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-claim-name-schema.json
slug: cognito-identity-claim-name
source_filename: cognito-identity-claim-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"[\\\\p{L}\\\\p{M}\\\\p{S}\\\\p{N}\\\\p{P}]+\",\n  \"minLength\": 1,\n  \"maxLength\": 64,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-claim-name-schema.json\",\n  \"title\": \"ClaimName\",\n  \"description\": \"ClaimName schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-claim-name-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ClaimName
---
