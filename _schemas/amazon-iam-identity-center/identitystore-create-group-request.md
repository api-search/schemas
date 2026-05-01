---
description: CreateGroupRequest schema from AWS IAM Identity Center
layout: schema
name: CreateGroupRequest
properties_list:
- description: ''
  name: IdentityStoreId
  type: object
- description: ''
  name: DisplayName
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-create-group-request-schema.json
slug: identitystore-create-group-request
source_filename: identitystore-create-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-create-group-request-schema.json\",\n  \"title\": \"CreateGroupRequest\",\n  \"description\": \"CreateGroupRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    },\n    \"DisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupDisplayName\"\n        },\n        {\n          \"description\": \"A string containing the name of the group. This value is commonly displayed when the group is referenced. \\\"Administrator\\\" and \\\"AWSAdministrators\\\"\
  \ are reserved names and can't be used for users or groups.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing the description of the group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityStoreId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-create-group-request-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: CreateGroupRequest
---
