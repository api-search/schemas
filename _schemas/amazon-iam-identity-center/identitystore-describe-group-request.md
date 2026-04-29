---
description: DescribeGroupRequest schema from AWS IAM Identity Center
layout: schema
name: DescribeGroupRequest
properties_list:
- description: ''
  name: IdentityStoreId
  type: object
- description: ''
  name: GroupId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-describe-group-request-schema.json
slug: identitystore-describe-group-request
source_filename: identitystore-describe-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-describe-group-request-schema.json\",\n  \"title\": \"DescribeGroupRequest\",\n  \"description\": \"DescribeGroupRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store, such as <code>d-1234567890</code>. In this example, <code>d-</code> is a fixed prefix, and <code>1234567890</code> is a randomly generated string that contains numbers and lower case letters. This value is generated at the time that a new identity store is created.\"\n        }\n      ]\n    },\n    \"GroupId\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for a group in the identity store.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityStoreId\",\n    \"GroupId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-describe-group-request-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: DescribeGroupRequest
---
