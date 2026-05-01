---
description: GetUICustomizationRequest schema from Amazon Cognito API
layout: schema
name: GetUICustomizationRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-ui-customization-request-schema.json
slug: user-pools-get-ui-customization-request
source_filename: user-pools-get-ui-customization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-ui-customization-request-schema.json\",\n  \"title\": \"GetUICustomizationRequest\",\n  \"description\": \"GetUICustomizationRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The client ID for the client app.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-ui-customization-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: GetUICustomizationRequest
---
