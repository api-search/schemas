---
description: ListGroupsRequest schema from Amazon Cognito API
layout: schema
name: ListGroupsRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Limit
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-groups-request-schema.json
slug: user-pools-list-groups-request
source_filename: user-pools-list-groups-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-groups-request-schema.json\",\n  \"title\": \"ListGroupsRequest\",\n  \"description\": \"ListGroupsRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryLimitType\"\n        },\n        {\n          \"description\": \"The limit of the request to list groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n     \
  \     \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-groups-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ListGroupsRequest
---
