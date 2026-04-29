---
description: IdentitiesList schema from Amazon Cognito
layout: schema
name: IdentitiesList
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-identities-list-schema.json
slug: cognito-identity-identities-list
source_filename: cognito-identity-identities-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"IdentityId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IdentityId\"\n          },\n          {\n            \"description\": \"A unique identifier in the format REGION:GUID.\"\n          }\n        ]\n      },\n      \"Logins\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/LoginsList\"\n          },\n          {\n            \"description\": \"The provider names.\"\n          }\n        ]\n      },\n      \"CreationDate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DateType\"\n          },\n          {\n            \"description\": \"Date on which the identity was created.\"\n          }\n        ]\n      },\n      \"LastModifiedDate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DateType\"\n          },\n          {\n\
  \            \"description\": \"Date on which the identity was last modified.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A description of the identity.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identities-list-schema.json\",\n  \"title\": \"IdentitiesList\",\n  \"description\": \"IdentitiesList schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-identities-list-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: IdentitiesList
---
