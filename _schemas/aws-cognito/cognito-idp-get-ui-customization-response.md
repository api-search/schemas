---
description: GetUICustomizationResponse schema from Amazon Cognito
layout: schema
name: GetUICustomizationResponse
properties_list:
- description: ''
  name: UICustomization
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-get-ui-customization-response-schema.json
slug: cognito-idp-get-ui-customization-response
source_filename: cognito-idp-get-ui-customization-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UICustomization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UICustomizationType\"\n        },\n        {\n          \"description\": \"The UI customization information.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UICustomization\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-ui-customization-response-schema.json\",\n  \"title\": \"GetUICustomizationResponse\",\n  \"description\": \"GetUICustomizationResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-ui-customization-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetUICustomizationResponse
---
