---
description: CreateGroupResponse schema from AWS IAM Identity Center
layout: schema
name: CreateGroupResponse
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: IdentityStoreId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-create-group-response-schema.json
slug: identitystore-create-group-response
source_filename: identitystore-create-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-create-group-response-schema.json\",\n  \"title\": \"CreateGroupResponse\",\n  \"description\": \"CreateGroupResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier of the newly created group in the identity store.\"\n        }\n      ]\n    },\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GroupId\",\n    \"IdentityStoreId\"\n \
  \ ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-create-group-response-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: CreateGroupResponse
---
