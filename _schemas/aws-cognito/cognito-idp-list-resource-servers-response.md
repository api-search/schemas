---
description: ListResourceServersResponse schema from Amazon Cognito
layout: schema
name: ListResourceServersResponse
properties_list:
- description: ''
  name: ResourceServers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-resource-servers-response-schema.json
slug: cognito-idp-list-resource-servers-response
source_filename: cognito-idp-list-resource-servers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceServers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServersListType\"\n        },\n        {\n          \"description\": \"The resource servers.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceServers\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-resource-servers-response-schema.json\",\n  \"title\": \"ListResourceServersResponse\",\n  \"description\": \"ListResourceServersResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-resource-servers-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListResourceServersResponse
---
