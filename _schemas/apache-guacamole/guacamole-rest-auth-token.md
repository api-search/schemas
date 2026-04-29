---
description: Authentication token response from Guacamole login
layout: schema
name: AuthToken
properties_list:
- description: Session authentication token
  name: authToken
  type: string
- description: Authenticated username
  name: username
  type: string
- description: Default data source identifier
  name: dataSource
  type: string
- description: List of available data source identifiers
  name: availableDataSources
  type: array
provider_name: Apache Guacamole
provider_slug: apache-guacamole
schema_file: json-schema/guacamole-rest-auth-token-schema.json
slug: guacamole-rest-auth-token
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-auth-token-schema.json\",\n  \"title\": \"AuthToken\",\n  \"description\": \"Authentication token response from Guacamole login\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authToken\": {\n      \"type\": \"string\",\n      \"description\": \"Session authentication token\",\n      \"example\": \"abc123def456\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Authenticated username\",\n      \"example\": \"guacadmin\"\n    },\n    \"dataSource\": {\n      \"type\": \"string\",\n      \"description\": \"Default data source identifier\",\n      \"example\": \"postgresql\"\n    },\n    \"availableDataSources\": {\n      \"type\": \"array\",\n      \"description\": \"List of available data source identifiers\",\n      \"items\": {\n        \"type\"\
  : \"string\"\n      },\n      \"example\": [\n        \"postgresql\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/json-schema/guacamole-rest-auth-token-schema.json
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
title: AuthToken
---
