---
description: The response from the server when Amazon Cognito makes the request to resend a confirmation code.
layout: schema
name: ResendConfirmationCodeResponse
properties_list:
- description: ''
  name: CodeDeliveryDetails
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-resend-confirmation-code-response-schema.json
slug: user-pools-resend-confirmation-code-response
source_filename: user-pools-resend-confirmation-code-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-resend-confirmation-code-response-schema.json\",\n  \"title\": \"ResendConfirmationCodeResponse\",\n  \"description\": \"The response from the server when Amazon Cognito makes the request to resend a confirmation code.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeDeliveryDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeDeliveryDetailsType\"\n        },\n        {\n          \"description\": \"The code delivery details returned by the server in response to the request to resend the confirmation code.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-resend-confirmation-code-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ResendConfirmationCodeResponse
---
