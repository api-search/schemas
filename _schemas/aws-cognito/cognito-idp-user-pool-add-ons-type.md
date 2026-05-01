---
description: The user pool add-ons type.
layout: schema
name: UserPoolAddOnsType
properties_list:
- description: ''
  name: AdvancedSecurityMode
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-user-pool-add-ons-type-schema.json
slug: cognito-idp-user-pool-add-ons-type
source_filename: cognito-idp-user-pool-add-ons-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdvancedSecurityMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedSecurityModeType\"\n        },\n        {\n          \"description\": \"The advanced security mode.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AdvancedSecurityMode\"\n  ],\n  \"description\": \"The user pool add-ons type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-pool-add-ons-type-schema.json\",\n  \"title\": \"UserPoolAddOnsType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-pool-add-ons-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UserPoolAddOnsType
---
