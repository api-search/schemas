---
description: The group type.
layout: schema
name: GroupType
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
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: CreationDate
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-group-type-schema.json
slug: user-pools-group-type
source_filename: user-pools-group-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-group-type-schema.json\",\n  \"title\": \"GroupType\",\n  \"description\": \"The group type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupNameType\"\n        },\n        {\n          \"description\": \"The name of the group.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionType\"\n        },\n        {\n          \"description\": \"A string containing the description of\
  \ the group.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The role Amazon Resource Name (ARN) for the group.\"\n        }\n      ]\n    },\n    \"Precedence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrecedenceType\"\n        },\n        {\n          \"description\": \"<p>A non-negative integer value that specifies the precedence of this group relative to the other groups that a user can belong to in the user pool. Zero is the highest precedence value. Groups with lower <code>Precedence</code> values take precedence over groups with higher ornull <code>Precedence</code> values. If a user belongs to two or more groups, it is the group with the lowest precedence value whose role ARN is given in the user's tokens for the <code>cognito:roles</code> and <code>cognito:preferred_role</code> claims.</p> <p>Two groups\
  \ can have the same <code>Precedence</code> value. If this happens, neither group takes precedence over the other. If two groups with the same <code>Precedence</code> have the same role ARN, that role is used in the <code>cognito:preferred_role</code> claim in tokens for users in each group. If the two groups have different role ARNs, the <code>cognito:preferred_role</code> claim isn't set in users' tokens.</p> <p>The default <code>Precedence</code> value is null.</p>\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was modified.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\"\
  : \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-group-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: GroupType
---
