---
description: Represents the request to set user settings.
layout: schema
name: SetUserSettingsRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
- description: ''
  name: MFAOptions
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-set-user-settings-request-schema.json
slug: user-pools-set-user-settings-request
source_filename: user-pools-set-user-settings-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-set-user-settings-request-schema.json\",\n  \"title\": \"SetUserSettingsRequest\",\n  \"description\": \"Represents the request to set user settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose user settings you want to configure.\"\n        }\n      ]\n    },\n    \"MFAOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MFAOptionListType\"\n        },\n        {\n          \"description\": \"You can use this parameter only to set an SMS configuration that uses SMS for delivery.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"AccessToken\",\n    \"MFAOptions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-set-user-settings-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: SetUserSettingsRequest
---
