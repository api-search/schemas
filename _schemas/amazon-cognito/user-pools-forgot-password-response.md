---
description: The response from Amazon Cognito to a request to reset a password.
layout: schema
name: ForgotPasswordResponse
properties_list:
- description: ''
  name: CodeDeliveryDetails
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-forgot-password-response-schema.json
slug: user-pools-forgot-password-response
source_filename: user-pools-forgot-password-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-forgot-password-response-schema.json\",\n  \"title\": \"ForgotPasswordResponse\",\n  \"description\": \"The response from Amazon Cognito to a request to reset a password.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeDeliveryDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeDeliveryDetailsType\"\n        },\n        {\n          \"description\": \"The code delivery details returned by the server in response to the request to reset a password.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-forgot-password-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ForgotPasswordResponse
---
