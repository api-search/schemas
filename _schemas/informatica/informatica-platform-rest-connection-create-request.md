---
description: Request body for creating a new connection.
layout: schema
name: ConnectionCreateRequest
properties_list:
- description: The resource type identifier. Must be set to "connection".
  name: '@type'
  type: string
- description: The name for the new connection.
  name: name
  type: string
- description: A description of the connection.
  name: description
  type: string
- description: The connection type.
  name: type
  type: string
- description: The runtime environment ID for the connection.
  name: runtimeEnvironmentId
  type: string
- description: The hostname or IP address.
  name: host
  type: string
- description: The port number.
  name: port
  type: integer
- description: The database name or service name.
  name: database
  type: string
- description: The database schema.
  name: schema
  type: string
- description: The username for authentication.
  name: username
  type: string
- description: The password for authentication.
  name: password
  type: string
- description: The authentication method.
  name: authenticationType
  type: string
- description: The service endpoint URL.
  name: serviceUrl
  type: string
- description: The character encoding.
  name: codepage
  type: string
- description: Additional connection-type-specific parameters.
  name: connParams
  type: object
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-connection-create-request-schema.json
slug: informatica-platform-rest-connection-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectionCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new connection.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier. Must be set to \\\"connection\\\".\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the new connection.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the connection.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The connection type.\"\n    },\n    \"runtimeEnvironmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime environment ID for the connection.\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname or IP address.\"\n    },\n    \"port\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"The port number.\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"The database name or service name.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"The database schema.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username for authentication.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The password for authentication.\"\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication method.\"\n    },\n    \"serviceUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The service endpoint URL.\"\n    },\n    \"codepage\": {\n      \"type\": \"string\",\n      \"description\": \"The character encoding.\"\n    },\n    \"connParams\": {\n      \"type\": \"object\",\n      \"description\": \"Additional connection-type-specific\
  \ parameters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-connection-create-request-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: ConnectionCreateRequest
---
