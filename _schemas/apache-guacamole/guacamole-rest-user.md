---
description: Guacamole user account
layout: schema
name: User
properties_list:
- description: Unique username
  name: username
  type: string
- description: User password (write-only)
  name: password
  type: string
- description: Additional user attributes
  name: attributes
  type: object
- description: Timestamp of last user activity in milliseconds
  name: lastActive
  type: integer
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-user-schema.json
slug: guacamole-rest-user
source_filename: guacamole-rest-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"Guacamole user account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Unique username\",\n      \"example\": \"jsmith\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"User password (write-only)\",\n      \"example\": \"securepassword123\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Additional user attributes\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"lastActive\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp of last user activity in milliseconds\",\n      \"example\"\
  : \"1718153645993\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-user-schema.json
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: User
---
