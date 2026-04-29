---
description: DescribeGroupMembershipResponse schema from AWS IAM Identity Center
layout: schema
name: DescribeGroupMembershipResponse
properties_list:
- description: ''
  name: IdentityStoreId
  type: object
- description: ''
  name: MembershipId
  type: object
- description: ''
  name: GroupId
  type: object
- description: An object containing the identifier of a group member.
  name: MemberId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-describe-group-membership-response-schema.json
slug: identitystore-describe-group-membership-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-describe-group-membership-response-schema.json\",\n  \"title\": \"DescribeGroupMembershipResponse\",\n  \"description\": \"DescribeGroupMembershipResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    },\n    \"MembershipId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for a <code>GroupMembership</code> in an identity store.\"\n        }\n      ]\n    },\n    \"GroupId\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for a group in the identity store.\"\n        }\n      ]\n    },\n    \"MemberId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"UserId\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ResourceId\"\n            },\n            {\n              \"description\": \"An object containing the identifiers of resources that can be members.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"An object containing the identifier of a group member.\"\n    }\n  },\n  \"required\": [\n    \"IdentityStoreId\",\n    \"MembershipId\",\n    \"GroupId\",\n    \"MemberId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-describe-group-membership-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: DescribeGroupMembershipResponse
---
