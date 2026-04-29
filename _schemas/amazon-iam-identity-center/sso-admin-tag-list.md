---
description: TagList schema from AWS IAM Identity Center
layout: schema
name: TagList
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-tag-list-schema.json
slug: sso-admin-tag-list
source_filename: sso-admin-tag-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-tag-list-schema.json\",\n  \"title\": \"TagList\",\n  \"description\": \"TagList schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"Key\",\n      \"Value\"\n    ],\n    \"properties\": {\n      \"Key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagKey\"\n          },\n          {\n            \"description\": \"The key for the tag.\"\n          }\n        ]\n      },\n      \"Value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TagValue\"\n          },\n          {\n            \"description\": \"The value of the tag.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A set of key-value pairs that are used\
  \ to manage the resource. Tags can only be applied to permission sets and cannot be applied to corresponding roles that IAM Identity Center creates in AWS accounts.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-tag-list-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: TagList
---
