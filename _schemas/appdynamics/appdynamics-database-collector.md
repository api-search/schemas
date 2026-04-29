---
description: Schema representing an AppDynamics Database Visibility collector configuration for monitoring database instances.
layout: schema
name: AppDynamics Database Collector
properties_list:
- description: The internal configuration ID for the database collector.
  name: id
  type: integer
- description: The display name for the database collector.
  name: name
  type: string
- description: The type of database being monitored.
  name: type
  type: string
- description: The hostname or IP address of the database server.
  name: hostname
  type: string
- description: The port number for the database connection.
  name: port
  type: integer
- description: The username for authenticating with the database.
  name: username
  type: string
- description: The password for authenticating with the database. Only used in create and update requests.
  name: password
  type: string
- description: The name of the specific database to monitor.
  name: databaseName
  type: string
- description: Whether the database collector is enabled and actively monitoring.
  name: enabled
  type: boolean
- description: The name of the Database Agent responsible for this collector.
  name: agentName
  type: string
- description: List of schema names to exclude from monitoring.
  name: excludedSchemas
  type: array
provider_name: AppDynamics
provider_slug: appdynamics
schema_file: json-schema/appdynamics-database-collector-schema.json
slug: appdynamics-database-collector
source_filename: appdynamics-database-collector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://appdynamics.com/schemas/appdynamics/database-collector.json\",\n  \"title\": \"AppDynamics Database Collector\",\n  \"description\": \"Schema representing an AppDynamics Database Visibility collector configuration for monitoring database instances.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\", \"hostname\", \"port\", \"username\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The internal configuration ID for the database collector.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the database collector.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of database being monitored.\",\n      \"enum\": [\n        \"MYSQL\",\n        \"ORACLE\",\n        \"MSSQL\",\n        \"\
  POSTGRESQL\",\n        \"MONGODB\",\n        \"SYBASE\",\n        \"DB2\",\n        \"AURORA\"\n      ]\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname or IP address of the database server.\",\n      \"minLength\": 1\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number for the database connection.\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username for authenticating with the database.\",\n      \"minLength\": 1\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The password for authenticating with the database. Only used in create and update requests.\"\n    },\n    \"databaseName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the specific database to monitor.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether the database collector is enabled and actively monitoring.\",\n      \"default\": true\n    },\n    \"agentName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Database Agent responsible for this collector.\"\n    },\n    \"excludedSchemas\": {\n      \"type\": \"array\",\n      \"description\": \"List of schema names to exclude from monitoring.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/json-schema/appdynamics-database-collector-schema.json
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
title: AppDynamics Database Collector
---
