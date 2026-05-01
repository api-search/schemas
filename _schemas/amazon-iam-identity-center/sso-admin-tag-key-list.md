---
description: TagKeyList schema from AWS IAM Identity Center
layout: schema
name: TagKeyList
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-tag-key-list-schema.json
slug: sso-admin-tag-key-list
source_filename: sso-admin-tag-key-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-tag-key-list-schema.json\",\n  \"title\": \"TagKeyList\",\n  \"description\": \"TagKeyList schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^([\\\\p{L}\\\\p{Z}\\\\p{N}_.:/=+\\\\-@]*)$\",\n    \"minLength\": 1,\n    \"maxLength\": 128\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-tag-key-list-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: TagKeyList
---
