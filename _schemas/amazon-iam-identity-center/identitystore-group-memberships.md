---
description: GroupMemberships schema from AWS IAM Identity Center
layout: schema
name: GroupMemberships
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-group-memberships-schema.json
slug: identitystore-group-memberships
source_filename: identitystore-group-memberships-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-group-memberships-schema.json\",\n  \"title\": \"GroupMemberships\",\n  \"description\": \"GroupMemberships schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"IdentityStoreId\"\n    ],\n    \"properties\": {\n      \"IdentityStoreId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IdentityStoreId\"\n          },\n          {\n            \"description\": \"The globally unique identifier for the identity store.\"\n          }\n        ]\n      },\n      \"MembershipId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceId\"\n          },\n          {\n            \"description\": \"The identifier for a <code>GroupMembership</code>\
  \ object in an identity store.\"\n          }\n        ]\n      },\n      \"GroupId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceId\"\n          },\n          {\n            \"description\": \"The identifier for a group in the identity store.\"\n          }\n        ]\n      },\n      \"MemberId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/MemberId\"\n          },\n          {\n            \"description\": \"An object that contains the identifier of a group member. Setting the <code>UserID</code> field to the specific identifier for a user indicates that the user is a member of the group.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains the identifiers for a group, a group member, and a <code>GroupMembership</code> object in the identity store.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-group-memberships-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: GroupMemberships
---
