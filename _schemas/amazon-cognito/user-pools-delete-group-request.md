---
description: DeleteGroupRequest schema from Amazon Cognito API
layout: schema
name: DeleteGroupRequest
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-delete-group-request-schema.json
slug: user-pools-delete-group-request
source_filename: user-pools-delete-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-group-request-schema.json\",\n  \"title\": \"DeleteGroupRequest\",\n  \"description\": \"DeleteGroupRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupNameType\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GroupName\",\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-group-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DeleteGroupRequest
---
