---
description: Represents the request to delete user attributes as an administrator.
layout: schema
name: AdminDeleteUserAttributesRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: UserAttributeNames
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-delete-user-attributes-request-schema.json
slug: cognito-idp-admin-delete-user-attributes-request
source_filename: cognito-idp-admin-delete-user-attributes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool where you want to delete user attributes.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user name of the user from which you would like to delete attributes.\"\n        }\n      ]\n    },\n    \"UserAttributeNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeNameListType\"\n        },\n        {\n          \"description\": \"<p>An array of strings representing the user attribute names you want to delete.</p> <p>For custom attributes, you must prepend the <code>custom:</code> prefix to the attribute name.</p>\"\n        }\n      ]\n   \
  \ }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Username\",\n    \"UserAttributeNames\"\n  ],\n  \"description\": \"Represents the request to delete user attributes as an administrator.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-delete-user-attributes-request-schema.json\",\n  \"title\": \"AdminDeleteUserAttributesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-delete-user-attributes-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminDeleteUserAttributesRequest
---
