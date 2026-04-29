---
description: Returned in response to a successful <code>GetCredentialsForIdentity</code> operation.
layout: schema
name: GetCredentialsForIdentityResponse
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Credentials
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-get-credentials-for-identity-response-schema.json
slug: identity-pools-get-credentials-for-identity-response
source_filename: identity-pools-get-credentials-for-identity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-get-credentials-for-identity-response-schema.json\",\n  \"title\": \"GetCredentialsForIdentityResponse\",\n  \"description\": \"Returned in response to a successful <code>GetCredentialsForIdentity</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Credentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Credentials\"\n        },\n        {\n          \"description\": \"Credentials for the provided identity ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-get-credentials-for-identity-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetCredentialsForIdentityResponse
---
