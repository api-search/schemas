---
description: ListGroupsResponse schema from Amazon Cognito
layout: schema
name: ListGroupsResponse
properties_list:
- description: ''
  name: Groups
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-groups-response-schema.json
slug: cognito-idp-list-groups-response
source_filename: cognito-idp-list-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupListType\"\n        },\n        {\n          \"description\": \"The group objects for the groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-groups-response-schema.json\",\n  \"title\": \"ListGroupsResponse\",\n  \"description\": \"ListGroupsResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-groups-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListGroupsResponse
---
