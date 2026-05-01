---
description: GroupMembershipExistenceResults schema from AWS IAM Identity Center
layout: schema
name: GroupMembershipExistenceResults
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-group-membership-existence-results-schema.json
slug: identitystore-group-membership-existence-results
source_filename: identitystore-group-membership-existence-results-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-group-membership-existence-results-schema.json\",\n  \"title\": \"GroupMembershipExistenceResults\",\n  \"description\": \"GroupMembershipExistenceResults schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"GroupId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceId\"\n          },\n          {\n            \"description\": \"The identifier for a group in the identity store.\"\n          }\n        ]\n      },\n      \"MemberId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/MemberId\"\n          },\n          {\n            \"description\": \"An object that contains the identifier of a group member. Setting the\
  \ <code>UserID</code> field to the specific identifier for a user indicates that the user is a member of the group.\"\n          }\n        ]\n      },\n      \"MembershipExists\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveBooleanType\"\n          },\n          {\n            \"description\": \"Indicates whether a membership relation exists or not.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Indicates whether a resource is a member of a group in the identity store.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-group-membership-existence-results-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: GroupMembershipExistenceResults
---
