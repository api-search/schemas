---
description: Policy item defining access permissions
layout: schema
name: PolicyItem
properties_list:
- description: Users granted access
  name: users
  type: array
- description: Groups granted access
  name: groups
  type: array
- description: ''
  name: accesses
  type: array
- description: ''
  name: conditions
  type: array
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-policy-item-schema.json
slug: apache-ranger-policy-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-policy-item-schema.json\",\n  \"title\": \"PolicyItem\",\n  \"description\": \"Policy item defining access permissions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Users granted access\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Groups granted access\"\n    },\n    \"accesses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AccessType\"\n      }\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-policy-item-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: PolicyItem
---
