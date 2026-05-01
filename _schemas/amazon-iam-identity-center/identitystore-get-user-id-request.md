---
description: GetUserIdRequest schema from AWS IAM Identity Center
layout: schema
name: GetUserIdRequest
properties_list:
- description: ''
  name: IdentityStoreId
  type: object
- description: ''
  name: AlternateIdentifier
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-get-user-id-request-schema.json
slug: identitystore-get-user-id-request
source_filename: identitystore-get-user-id-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-get-user-id-request-schema.json\",\n  \"title\": \"GetUserIdRequest\",\n  \"description\": \"GetUserIdRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    },\n    \"AlternateIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlternateIdentifier\"\n        },\n        {\n          \"description\": \"A unique identifier for a user or group that is not the primary identifier. This value can be an identifier from an external identity provider (IdP) that\
  \ is associated with the user, the group, or a unique attribute. For the unique attribute, the only valid paths are <code>userName</code> and <code>emails.value</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityStoreId\",\n    \"AlternateIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-get-user-id-request-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: GetUserIdRequest
---
