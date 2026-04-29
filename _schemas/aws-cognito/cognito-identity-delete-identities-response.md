---
description: Returned in response to a successful <code>DeleteIdentities</code> operation.
layout: schema
name: DeleteIdentitiesResponse
properties_list:
- description: ''
  name: UnprocessedIdentityIds
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-delete-identities-response-schema.json
slug: cognito-identity-delete-identities-response
source_filename: cognito-identity-delete-identities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnprocessedIdentityIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedIdentityIdList\"\n        },\n        {\n          \"description\": \"An array of UnprocessedIdentityId objects, each of which contains an ErrorCode and IdentityId.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Returned in response to a successful <code>DeleteIdentities</code> operation.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-delete-identities-response-schema.json\",\n  \"title\": \"DeleteIdentitiesResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-delete-identities-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeleteIdentitiesResponse
---
