---
description: ''
layout: schema
name: LoggingConfig
properties_list:
- description: Log output directory
  name: logDirectory
  type: string
- description: ''
  name: consoleLogLevel
  type: string
- description: Name of the messages log file
  name: messageFileName
  type: string
- description: Name of the trace log file
  name: traceFileName
  type: string
- description: Trace specification string
  name: traceSpecification
  type: string
- description: Maximum log file size in MB
  name: maxFileSize
  type: integer
- description: Maximum number of log files
  name: maxFiles
  type: integer
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-admin-rest-logging-config-schema.json
slug: websphere-liberty-admin-rest-logging-config
source_filename: websphere-liberty-admin-rest-logging-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoggingConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Log output directory\"\n    },\n    \"consoleLogLevel\": {\n      \"type\": \"string\"\n    },\n    \"messageFileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the messages log file\"\n    },\n    \"traceFileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the trace log file\"\n    },\n    \"traceSpecification\": {\n      \"type\": \"string\",\n      \"description\": \"Trace specification string\"\n    },\n    \"maxFileSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum log file size in MB\"\n    },\n    \"maxFiles\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of log files\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-admin-rest-logging-config-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: LoggingConfig
---
