---
description: Represents the request to delete user attributes.
layout: schema
name: DeleteUserAttributesRequest
properties_list:
- description: ''
  name: UserAttributeNames
  type: object
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-delete-user-attributes-request-schema.json
slug: cognito-idp-delete-user-attributes-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserAttributeNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeNameListType\"\n        },\n        {\n          \"description\": \"<p>An array of strings representing the user attribute names you want to delete.</p> <p>For custom attributes, you must prependattach the <code>custom:</code> prefix to the front of the attribute name.</p>\"\n        }\n      ]\n    },\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose attributes you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserAttributeNames\",\n    \"AccessToken\"\n  ],\n  \"description\": \"Represents the request to delete user attributes.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"\
  $id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-user-attributes-request-schema.json\",\n  \"title\": \"DeleteUserAttributesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-delete-user-attributes-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: DeleteUserAttributesRequest
---
