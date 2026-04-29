---
description: Represents a connection to a data source or target in Informatica Intelligent Cloud Services.
layout: schema
name: Connection
properties_list:
- description: The resource type identifier.
  name: '@type'
  type: string
- description: The unique identifier for the connection.
  name: id
  type: string
- description: The organization ID that owns the connection.
  name: orgId
  type: string
- description: The name of the connection.
  name: name
  type: string
- description: A description of the connection.
  name: description
  type: string
- description: The connection type (e.g., Oracle, Salesforce, MySQL, SqlServer, FTP, CSVFile).
  name: type
  type: string
- description: The time the connection was created.
  name: createTime
  type: string
- description: The time the connection was last updated.
  name: updateTime
  type: string
- description: The user who created the connection.
  name: createdBy
  type: string
- description: The user who last updated the connection.
  name: updatedBy
  type: string
- description: The ID of the Secure Agent associated with the connection.
  name: agentId
  type: string
- description: The ID of the runtime environment associated with the connection.
  name: runtimeEnvironmentId
  type: string
- description: The hostname or IP address for the connection. Applicable to database and server-based connections.
  name: host
  type: string
- description: The port number for the connection. Applicable to database and server-based connections.
  name: port
  type: integer
- description: The database name or service name for the connection.
  name: database
  type: string
- description: The database schema name.
  name: schema
  type: string
- description: The username for authentication.
  name: username
  type: string
- description: The password for authentication.
  name: password
  type: string
- description: The authentication method used by the connection.
  name: authenticationType
  type: string
- description: The service endpoint URL. Applicable to web service and cloud application connections.
  name: serviceUrl
  type: string
- description: The character encoding for the connection (e.g., UTF-8).
  name: codepage
  type: string
- description: Additional connection parameters specific to the connection type. Contains attributes not listed as top-level fields.
  name: connParams
  type: object
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-connection-schema.json
slug: informatica-platform-rest-connection
source_filename: informatica-platform-rest-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Connection\",\n  \"type\": \"object\",\n  \"description\": \"Represents a connection to a data source or target in Informatica Intelligent Cloud Services.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the connection.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"The organization ID that owns the connection.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the connection.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the connection.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The connection type (e.g., Oracle, Salesforce, MySQL, SqlServer,\
  \ FTP, CSVFile).\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the connection was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the connection was last updated.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the connection.\"\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last updated the connection.\"\n    },\n    \"agentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Secure Agent associated with the connection.\"\n    },\n    \"runtimeEnvironmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the runtime environment associated with the connection.\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname or IP address for the connection. Applicable to database and server-based\
  \ connections.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number for the connection. Applicable to database and server-based connections.\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"The database name or service name for the connection.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"The database schema name.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username for authentication.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The password for authentication.\"\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication method used by the connection.\"\n    },\n    \"serviceUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The service endpoint URL. Applicable to web service and cloud application connections.\"\n\
  \    },\n    \"codepage\": {\n      \"type\": \"string\",\n      \"description\": \"The character encoding for the connection (e.g., UTF-8).\"\n    },\n    \"connParams\": {\n      \"type\": \"object\",\n      \"description\": \"Additional connection parameters specific to the connection type. Contains attributes not listed as top-level fields.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-connection-schema.json
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
title: Connection
---
