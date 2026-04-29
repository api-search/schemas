---
description: UpdateGroupRequest schema from Amazon Cognito API
layout: schema
name: UpdateGroupRequest
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Precedence
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-update-group-request-schema.json
slug: user-pools-update-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-group-request-schema.json\",\n  \"title\": \"UpdateGroupRequest\",\n  \"description\": \"UpdateGroupRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupNameType\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionType\"\n        },\n        {\n          \"description\"\
  : \"A string containing the new description of the group.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The new role Amazon Resource Name (ARN) for the group. This is used for setting the <code>cognito:roles</code> and <code>cognito:preferred_role</code> claims in the token.\"\n        }\n      ]\n    },\n    \"Precedence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrecedenceType\"\n        },\n        {\n          \"description\": \"The new precedence value for the group. For more information about this parameter, see <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_CreateGroup.html\\\">CreateGroup</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GroupName\",\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-update-group-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UpdateGroupRequest
---
