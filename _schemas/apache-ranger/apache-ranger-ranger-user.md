---
description: Ranger user definition
layout: schema
name: RangerUser
properties_list:
- description: User identifier
  name: id
  type: integer
- description: Username
  name: name
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: emailAddress
  type: string
- description: User source (0=internal, 1=LDAP/AD)
  name: userSource
  type: integer
- description: User status (1=active, 0=disabled)
  name: status
  type: integer
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-ranger-user-schema.json
slug: apache-ranger-ranger-user
source_filename: apache-ranger-ranger-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-ranger-user-schema.json\",\n  \"title\": \"RangerUser\",\n  \"description\": \"Ranger user definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"User identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Username\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"emailAddress\": {\n      \"type\": \"string\"\n    },\n    \"userSource\": {\n      \"type\": \"integer\",\n      \"description\": \"User source (0=internal, 1=LDAP/AD)\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"User status (1=active, 0=disabled)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-ranger-user-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: RangerUser
---
