---
description: SetUICustomizationRequest schema from Amazon Cognito
layout: schema
name: SetUICustomizationRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientId
  type: object
- description: ''
  name: CSS
  type: object
- description: ''
  name: ImageFile
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-set-ui-customization-request-schema.json
slug: cognito-idp-set-ui-customization-request
source_filename: cognito-idp-set-ui-customization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The client ID for the client app.\"\n        }\n      ]\n    },\n    \"CSS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CSSType\"\n        },\n        {\n          \"description\": \"The CSS values in the UI customization.\"\n        }\n      ]\n    },\n    \"ImageFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageFileType\"\n        },\n        {\n          \"description\": \"The uploaded logo image for the UI customization.\"\n        }\n      ]\n    }\n  },\n \
  \ \"required\": [\n    \"UserPoolId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-set-ui-customization-request-schema.json\",\n  \"title\": \"SetUICustomizationRequest\",\n  \"description\": \"SetUICustomizationRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-set-ui-customization-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SetUICustomizationRequest
---
