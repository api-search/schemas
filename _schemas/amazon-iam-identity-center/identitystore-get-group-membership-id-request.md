---
description: GetGroupMembershipIdRequest schema from AWS IAM Identity Center
layout: schema
name: GetGroupMembershipIdRequest
properties_list:
- description: ''
  name: IdentityStoreId
  type: object
- description: ''
  name: GroupId
  type: object
- description: ''
  name: MemberId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-get-group-membership-id-request-schema.json
slug: identitystore-get-group-membership-id-request
source_filename: identitystore-get-group-membership-id-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-get-group-membership-id-request-schema.json\",\n  \"title\": \"GetGroupMembershipIdRequest\",\n  \"description\": \"GetGroupMembershipIdRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    },\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for a group in the identity store.\"\n        }\n      ]\n    },\n    \"MemberId\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/MemberId\"\n        },\n        {\n          \"description\": \"An object that contains the identifier of a group member. Setting the <code>UserID</code> field to the specific identifier for a user indicates that the user is a member of the group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityStoreId\",\n    \"GroupId\",\n    \"MemberId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-get-group-membership-id-request-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: GetGroupMembershipIdRequest
---
