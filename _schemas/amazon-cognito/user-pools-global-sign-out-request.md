---
description: Represents the request to sign out all devices.
layout: schema
name: GlobalSignOutRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-global-sign-out-request-schema.json
slug: user-pools-global-sign-out-request
source_filename: user-pools-global-sign-out-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-global-sign-out-request-schema.json\",\n  \"title\": \"GlobalSignOutRequest\",\n  \"description\": \"Represents the request to sign out all devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user who you want to sign out.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-global-sign-out-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GlobalSignOutRequest
---
