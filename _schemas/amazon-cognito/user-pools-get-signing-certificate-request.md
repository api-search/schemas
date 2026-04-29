---
description: Request to get a signing certificate from Amazon Cognito.
layout: schema
name: GetSigningCertificateRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-signing-certificate-request-schema.json
slug: user-pools-get-signing-certificate-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-signing-certificate-request-schema.json\",\n  \"title\": \"GetSigningCertificateRequest\",\n  \"description\": \"Request to get a signing certificate from Amazon Cognito.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-signing-certificate-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetSigningCertificateRequest
---
