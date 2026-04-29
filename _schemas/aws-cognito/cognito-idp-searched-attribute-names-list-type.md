---
description: SearchedAttributeNamesListType schema from Amazon Cognito
layout: schema
name: SearchedAttributeNamesListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-searched-attribute-names-list-type-schema.json
slug: cognito-idp-searched-attribute-names-list-type
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[\\\\p{L}\\\\p{M}\\\\p{S}\\\\p{N}\\\\p{P}]+\",\n    \"minLength\": 1,\n    \"maxLength\": 32\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-searched-attribute-names-list-type-schema.json\",\n  \"title\": \"SearchedAttributeNamesListType\",\n  \"description\": \"SearchedAttributeNamesListType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-searched-attribute-names-list-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SearchedAttributeNamesListType
---
