---
description: Represents the request to change a user password.
layout: schema
name: ChangePasswordRequest
properties_list:
- description: ''
  name: PreviousPassword
  type: object
- description: ''
  name: ProposedPassword
  type: object
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-change-password-request-schema.json
slug: user-pools-change-password-request
source_filename: user-pools-change-password-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-change-password-request-schema.json\",\n  \"title\": \"ChangePasswordRequest\",\n  \"description\": \"Represents the request to change a user password.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PreviousPassword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordType\"\n        },\n        {\n          \"description\": \"The old password.\"\n        }\n      ]\n    },\n    \"ProposedPassword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordType\"\n        },\n        {\n          \"description\": \"The new password.\"\n        }\n      ]\n    },\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\"\
  : \"A valid access token that Amazon Cognito issued to the user whose password you want to change.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PreviousPassword\",\n    \"ProposedPassword\",\n    \"AccessToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-change-password-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ChangePasswordRequest
---
