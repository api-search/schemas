---
description: Access audit log entries
layout: schema
name: AuditList
properties_list:
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: auditList
  type: array
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-audit-list-schema.json
slug: apache-ranger-audit-list
source_filename: apache-ranger-audit-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-audit-list-schema.json\",\n  \"title\": \"AuditList\",\n  \"description\": \"Access audit log entries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"auditList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AuditEntry\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-audit-list-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: AuditList
---
