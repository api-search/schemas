---
description: AccountList schema from AWS IAM Identity Center
layout: schema
name: AccountList
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-account-list-schema.json
slug: sso-admin-account-list
source_filename: sso-admin-account-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-account-list-schema.json\",\n  \"title\": \"AccountList\",\n  \"description\": \"AccountList schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"\\\\d{12}\",\n    \"minLength\": 12,\n    \"maxLength\": 12\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-account-list-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: AccountList
---
