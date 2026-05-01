---
description: The authentication result.
layout: schema
name: AuthenticationResultType
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: ExpiresIn
  type: object
- description: ''
  name: TokenType
  type: object
- description: ''
  name: RefreshToken
  type: object
- description: ''
  name: IdToken
  type: object
- description: ''
  name: NewDeviceMetadata
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-authentication-result-type-schema.json
slug: user-pools-authentication-result-type
source_filename: user-pools-authentication-result-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-authentication-result-type-schema.json\",\n  \"title\": \"AuthenticationResultType\",\n  \"description\": \"The authentication result.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user who you want to authenticate.\"\n        }\n      ]\n    },\n    \"ExpiresIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerType\"\n        },\n        {\n          \"description\": \"The expiration period of the authentication result in seconds.\"\n        }\n      ]\n    },\n    \"TokenType\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The token type.\"\n        }\n      ]\n    },\n    \"RefreshToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"The refresh token.\"\n        }\n      ]\n    },\n    \"IdToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"The ID token.\"\n        }\n      ]\n    },\n    \"NewDeviceMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NewDeviceMetadataType\"\n        },\n        {\n          \"description\": \"The new device metadata from an authentication result.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-authentication-result-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: AuthenticationResultType
---
