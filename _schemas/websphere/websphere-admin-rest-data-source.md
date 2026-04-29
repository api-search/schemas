---
description: ''
layout: schema
name: DataSource
properties_list:
- description: Data source name
  name: name
  type: string
- description: JNDI name
  name: jndiName
  type: string
- description: Database type
  name: databaseType
  type: string
- description: JDBC provider name
  name: jdbcProvider
  type: string
- description: ''
  name: connectionPool
  type: object
- description: ''
  name: status
  type: string
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-admin-rest-data-source-schema.json
slug: websphere-admin-rest-data-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Data source name\"\n    },\n    \"jndiName\": {\n      \"type\": \"string\",\n      \"description\": \"JNDI name\"\n    },\n    \"databaseType\": {\n      \"type\": \"string\",\n      \"description\": \"Database type\"\n    },\n    \"jdbcProvider\": {\n      \"type\": \"string\",\n      \"description\": \"JDBC provider name\"\n    },\n    \"connectionPool\": {\n      \"type\": \"object\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-admin-rest-data-source-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: DataSource
---
