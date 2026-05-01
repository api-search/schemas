---
description: DeleteGroupMembershipRequest schema from AWS IAM Identity Center
layout: schema
name: DeleteGroupMembershipRequest
properties_list:
- description: ''
  name: IdentityStoreId
  type: object
- description: ''
  name: MembershipId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-delete-group-membership-request-schema.json
slug: identitystore-delete-group-membership-request
source_filename: identitystore-delete-group-membership-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-delete-group-membership-request-schema.json\",\n  \"title\": \"DeleteGroupMembershipRequest\",\n  \"description\": \"DeleteGroupMembershipRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    },\n    \"MembershipId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for a <code>GroupMembership</code> in an identity store.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  IdentityStoreId\",\n    \"MembershipId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-delete-group-membership-request-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: DeleteGroupMembershipRequest
---
