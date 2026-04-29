---
description: Resource specification in a Ranger policy
layout: schema
name: PolicyResource
properties_list:
- description: Resource values (paths, tables, etc.)
  name: values
  type: array
- description: Whether to apply recursively
  name: isRecursive
  type: boolean
- description: Whether this is an exclusion list
  name: isExcludes
  type: boolean
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-policy-resource-schema.json
slug: apache-ranger-policy-resource
source_filename: apache-ranger-policy-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-policy-resource-schema.json\",\n  \"title\": \"PolicyResource\",\n  \"description\": \"Resource specification in a Ranger policy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Resource values (paths, tables, etc.)\"\n    },\n    \"isRecursive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to apply recursively\"\n    },\n    \"isExcludes\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an exclusion list\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-policy-resource-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: PolicyResource
---
