---
description: UpdateGroupRequest schema from AWS IAM Identity Center
layout: schema
name: UpdateGroupRequest
properties_list:
- description: ''
  name: IdentityStoreId
  type: object
- description: ''
  name: GroupId
  type: object
- description: ''
  name: Operations
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-update-group-request-schema.json
slug: identitystore-update-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-update-group-request-schema.json\",\n  \"title\": \"UpdateGroupRequest\",\n  \"description\": \"UpdateGroupRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    },\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for a group in the identity store.\"\n        }\n      ]\n    },\n    \"Operations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeOperations\"\
  \n        },\n        {\n          \"description\": \"A list of <code>AttributeOperation</code> objects to apply to the requested group. These operations might add, replace, or remove an attribute.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityStoreId\",\n    \"GroupId\",\n    \"Operations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-update-group-request-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: UpdateGroupRequest
---
