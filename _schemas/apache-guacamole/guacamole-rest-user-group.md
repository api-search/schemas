---
description: Guacamole user group for shared permissions
layout: schema
name: UserGroup
properties_list:
- description: Unique group identifier
  name: identifier
  type: string
- description: Group attributes
  name: attributes
  type: object
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-user-group-schema.json
slug: guacamole-rest-user-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-user-group-schema.json\",\n  \"title\": \"UserGroup\",\n  \"description\": \"Guacamole user group for shared permissions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique group identifier\",\n      \"example\": \"admins\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Group attributes\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-user-group-schema.json
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: UserGroup
---
