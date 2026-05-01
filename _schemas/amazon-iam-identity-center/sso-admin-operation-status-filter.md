---
description: Filters he operation status list based on the passed attribute value.
layout: schema
name: OperationStatusFilter
properties_list:
- description: ''
  name: Status
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-operation-status-filter-schema.json
slug: sso-admin-operation-status-filter
source_filename: sso-admin-operation-status-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-operation-status-filter-schema.json\",\n  \"title\": \"OperationStatusFilter\",\n  \"description\": \"Filters he operation status list based on the passed attribute value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusValues\"\n        },\n        {\n          \"description\": \"Filters the list operations result based on the status attribute.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-operation-status-filter-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: OperationStatusFilter
---
