---
description: Input to the UnlinkIdentity action.
layout: schema
name: UnlinkIdentityInput
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Logins
  type: object
- description: ''
  name: LoginsToRemove
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-unlink-identity-input-schema.json
slug: identity-pools-unlink-identity-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-unlink-identity-input-schema.json\",\n  \"title\": \"UnlinkIdentityInput\",\n  \"description\": \"Input to the UnlinkIdentity action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Logins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginsMap\"\n        },\n        {\n          \"description\": \"A set of optional name-value pairs that map provider names to provider tokens.\"\n        }\n      ]\n    },\n    \"LoginsToRemove\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginsList\"\
  \n        },\n        {\n          \"description\": \"Provider names to unlink from this identity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityId\",\n    \"Logins\",\n    \"LoginsToRemove\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-unlink-identity-input-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UnlinkIdentityInput
---
