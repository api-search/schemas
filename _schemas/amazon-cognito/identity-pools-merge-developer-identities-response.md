---
description: Returned in response to a successful <code>MergeDeveloperIdentities</code> action.
layout: schema
name: MergeDeveloperIdentitiesResponse
properties_list:
- description: ''
  name: IdentityId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-merge-developer-identities-response-schema.json
slug: identity-pools-merge-developer-identities-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-merge-developer-identities-response-schema.json\",\n  \"title\": \"MergeDeveloperIdentitiesResponse\",\n  \"description\": \"Returned in response to a successful <code>MergeDeveloperIdentities</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-merge-developer-identities-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: MergeDeveloperIdentitiesResponse
---
