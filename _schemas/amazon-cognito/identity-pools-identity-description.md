---
description: A description of the identity.
layout: schema
name: IdentityDescription
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: Logins
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: LastModifiedDate
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-identity-description-schema.json
slug: identity-pools-identity-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-identity-description-schema.json\",\n  \"title\": \"IdentityDescription\",\n  \"description\": \"A description of the identity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Logins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginsList\"\n        },\n        {\n          \"description\": \"The provider names.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"Date on\
  \ which the identity was created.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"Date on which the identity was last modified.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-identity-description-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: IdentityDescription
---
