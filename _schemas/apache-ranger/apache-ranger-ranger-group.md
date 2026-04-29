---
description: Ranger user group
layout: schema
name: RangerGroup
properties_list:
- description: Group identifier
  name: id
  type: integer
- description: Group name
  name: name
  type: string
- description: Group description
  name: description
  type: string
- description: Group source (0=internal, 1=LDAP/AD)
  name: groupSource
  type: integer
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-ranger-group-schema.json
slug: apache-ranger-ranger-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-ranger-group-schema.json\",\n  \"title\": \"RangerGroup\",\n  \"description\": \"Ranger user group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Group identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Group name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Group description\"\n    },\n    \"groupSource\": {\n      \"type\": \"integer\",\n      \"description\": \"Group source (0=internal, 1=LDAP/AD)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-ranger-group-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: RangerGroup
---
