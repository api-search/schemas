---
description: SecretHashType schema from Amazon Cognito
layout: schema
name: SecretHashType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-secret-hash-type-schema.json
slug: cognito-idp-secret-hash-type
source_filename: cognito-idp-secret-hash-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"[\\\\w+=/]+\",\n  \"minLength\": 1,\n  \"maxLength\": 128,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-secret-hash-type-schema.json\",\n  \"title\": \"SecretHashType\",\n  \"description\": \"SecretHashType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-secret-hash-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SecretHashType
---
