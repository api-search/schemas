---
description: AccessControlAttributeValueSourceList schema from AWS IAM Identity Center
layout: schema
name: AccessControlAttributeValueSourceList
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-access-control-attribute-value-source-list-schema.json
slug: sso-admin-access-control-attribute-value-source-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-access-control-attribute-value-source-list-schema.json\",\n  \"title\": \"AccessControlAttributeValueSourceList\",\n  \"description\": \"AccessControlAttributeValueSourceList schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"[\\\\p{L}\\\\p{Z}\\\\p{N}_.:\\\\/=+\\\\-@\\\\[\\\\]\\\\{\\\\}\\\\$\\\\\\\\\\\"]*\",\n    \"minLength\": 0,\n    \"maxLength\": 256\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-access-control-attribute-value-source-list-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: AccessControlAttributeValueSourceList
---
