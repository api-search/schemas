---
description: GetGroupMembershipIdResponse schema from AWS IAM Identity Center
layout: schema
name: GetGroupMembershipIdResponse
properties_list:
- description: ''
  name: MembershipId
  type: object
- description: ''
  name: IdentityStoreId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-get-group-membership-id-response-schema.json
slug: identitystore-get-group-membership-id-response
source_filename: identitystore-get-group-membership-id-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-get-group-membership-id-response-schema.json\",\n  \"title\": \"GetGroupMembershipIdResponse\",\n  \"description\": \"GetGroupMembershipIdResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MembershipId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for a <code>GroupMembership</code> in an identity store.\"\n        }\n      ]\n    },\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n   \
  \ \"MembershipId\",\n    \"IdentityStoreId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-get-group-membership-id-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: GetGroupMembershipIdResponse
---
