---
description: ExplicitAuthFlowsListType schema from Amazon Cognito
layout: schema
name: ExplicitAuthFlowsListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-explicit-auth-flows-list-type-schema.json
slug: cognito-idp-explicit-auth-flows-list-type
source_filename: cognito-idp-explicit-auth-flows-list-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"enum\": [\n      \"ADMIN_NO_SRP_AUTH\",\n      \"CUSTOM_AUTH_FLOW_ONLY\",\n      \"USER_PASSWORD_AUTH\",\n      \"ALLOW_ADMIN_USER_PASSWORD_AUTH\",\n      \"ALLOW_CUSTOM_AUTH\",\n      \"ALLOW_USER_PASSWORD_AUTH\",\n      \"ALLOW_USER_SRP_AUTH\",\n      \"ALLOW_REFRESH_TOKEN_AUTH\"\n    ]\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-explicit-auth-flows-list-type-schema.json\",\n  \"title\": \"ExplicitAuthFlowsListType\",\n  \"description\": \"ExplicitAuthFlowsListType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-explicit-auth-flows-list-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ExplicitAuthFlowsListType
---
