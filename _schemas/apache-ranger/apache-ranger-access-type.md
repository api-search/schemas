---
description: Access type in a policy item
layout: schema
name: AccessType
properties_list:
- description: Access type name (read, write, execute, etc.)
  name: type
  type: string
- description: Whether the access is allowed
  name: isAllowed
  type: boolean
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-access-type-schema.json
slug: apache-ranger-access-type
source_filename: apache-ranger-access-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-access-type-schema.json\",\n  \"title\": \"AccessType\",\n  \"description\": \"Access type in a policy item\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Access type name (read, write, execute, etc.)\"\n    },\n    \"isAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the access is allowed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-access-type-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: AccessType
---
