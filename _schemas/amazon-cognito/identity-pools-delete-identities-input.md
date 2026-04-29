---
description: Input to the <code>DeleteIdentities</code> action.
layout: schema
name: DeleteIdentitiesInput
properties_list:
- description: ''
  name: IdentityIdsToDelete
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-delete-identities-input-schema.json
slug: identity-pools-delete-identities-input
source_filename: identity-pools-delete-identities-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-delete-identities-input-schema.json\",\n  \"title\": \"DeleteIdentitiesInput\",\n  \"description\": \"Input to the <code>DeleteIdentities</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityIdsToDelete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityIdList\"\n        },\n        {\n          \"description\": \"A list of 1-60 identities that you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityIdsToDelete\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-delete-identities-input-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DeleteIdentitiesInput
---
