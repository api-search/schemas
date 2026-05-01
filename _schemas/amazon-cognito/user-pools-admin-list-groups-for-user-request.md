---
description: AdminListGroupsForUserRequest schema from Amazon Cognito API
layout: schema
name: AdminListGroupsForUserRequest
properties_list:
- description: ''
  name: Username
  type: object
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
schema_file: json-schema/user-pools-admin-list-groups-for-user-request-schema.json
slug: user-pools-admin-list-groups-for-user-request
source_filename: user-pools-admin-list-groups-for-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-list-groups-for-user-request-schema.json\",\n  \"title\": \"AdminListGroupsForUserRequest\",\n  \"description\": \"AdminListGroupsForUserRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The username for the user.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryLimitType\"\n     \
  \   },\n        {\n          \"description\": \"The limit of the request to list groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Username\",\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-list-groups-for-user-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: AdminListGroupsForUserRequest
---
