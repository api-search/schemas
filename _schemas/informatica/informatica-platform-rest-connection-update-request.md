---
description: Request body for updating an existing connection.
layout: schema
name: ConnectionUpdateRequest
properties_list:
- description: The resource type identifier. Must be set to "connection".
  name: '@type'
  type: string
- description: The updated name for the connection.
  name: name
  type: string
- description: An updated description of the connection.
  name: description
  type: string
- description: The updated hostname or IP address.
  name: host
  type: string
- description: The updated port number.
  name: port
  type: integer
- description: The updated database name.
  name: database
  type: string
- description: The updated database schema.
  name: schema
  type: string
- description: The updated username.
  name: username
  type: string
- description: The updated password.
  name: password
  type: string
- description: The updated authentication method.
  name: authenticationType
  type: string
- description: The updated service endpoint URL.
  name: serviceUrl
  type: string
- description: The updated character encoding.
  name: codepage
  type: string
- description: Updated connection-type-specific parameters.
  name: connParams
  type: object
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-connection-update-request-schema.json
slug: informatica-platform-rest-connection-update-request
source_filename: informatica-platform-rest-connection-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectionUpdateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an existing connection.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier. Must be set to \\\"connection\\\".\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The updated name for the connection.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An updated description of the connection.\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The updated hostname or IP address.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The updated port number.\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"The updated database name.\"\n    },\n    \"schema\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The updated database schema.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The updated username.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The updated password.\"\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"description\": \"The updated authentication method.\"\n    },\n    \"serviceUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The updated service endpoint URL.\"\n    },\n    \"codepage\": {\n      \"type\": \"string\",\n      \"description\": \"The updated character encoding.\"\n    },\n    \"connParams\": {\n      \"type\": \"object\",\n      \"description\": \"Updated connection-type-specific parameters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-connection-update-request-schema.json
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
title: ConnectionUpdateRequest
---
