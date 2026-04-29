---
description: ListGroupsResponse schema from Amazon Cognito API
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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-groups-response-schema.json
slug: user-pools-list-groups-response
source_filename: user-pools-list-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-groups-response-schema.json\",\n  \"title\": \"ListGroupsResponse\",\n  \"description\": \"ListGroupsResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupListType\"\n        },\n        {\n          \"description\": \"The group objects for the groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-groups-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListGroupsResponse
---
