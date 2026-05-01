---
description: A Lake Formation permission grant.
layout: schema
name: Permission
properties_list:
- description: The principal (IAM user, role, or group) being granted permissions.
  name: Principal
  type: object
- description: The resource on which permissions are being granted.
  name: Resource
  type: object
- description: The permissions being granted.
  name: Permissions
  type: array
provider_name: Amazon Lake Formation
provider_slug: amazon-lake-formation
schema_file: json-schema/amazon-lake-formation-permission-schema.json
slug: amazon-lake-formation-permission
source_filename: amazon-lake-formation-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lake-formation/refs/heads/main/json-schema/amazon-lake-formation-permission-schema.json\",\n  \"title\": \"Permission\",\n  \"description\": \"A Lake Formation permission grant.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Principal\": {\n      \"type\": \"object\",\n      \"description\": \"The principal (IAM user, role, or group) being granted permissions.\"\n    },\n    \"Resource\": {\n      \"type\": \"object\",\n      \"description\": \"The resource on which permissions are being granted.\"\n    },\n    \"Permissions\": {\n      \"type\": \"array\",\n      \"description\": \"The permissions being granted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lake-formation/refs/heads/main/json-schema/amazon-lake-formation-permission-schema.json
tags:
- Access Control
- Analytics
- Data Governance
- Data Lake
- S3
title: Permission
---
