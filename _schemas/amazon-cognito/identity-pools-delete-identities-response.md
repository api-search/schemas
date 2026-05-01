---
description: Returned in response to a successful <code>DeleteIdentities</code> operation.
layout: schema
name: DeleteIdentitiesResponse
properties_list:
- description: ''
  name: UnprocessedIdentityIds
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-delete-identities-response-schema.json
slug: identity-pools-delete-identities-response
source_filename: identity-pools-delete-identities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-delete-identities-response-schema.json\",\n  \"title\": \"DeleteIdentitiesResponse\",\n  \"description\": \"Returned in response to a successful <code>DeleteIdentities</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnprocessedIdentityIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedIdentityIdList\"\n        },\n        {\n          \"description\": \"An array of UnprocessedIdentityId objects, each of which contains an ErrorCode and IdentityId.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-delete-identities-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: DeleteIdentitiesResponse
---
