---
description: ''
layout: schema
name: DatabaseConnection
properties_list:
- description: Connection name
  name: name
  type: string
- description: Database type
  name: type
  type: string
- description: Database connection string
  name: connectionString
  type: string
- description: ''
  name: credentials
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-database-connection-schema.json
slug: oracle-goldengate-rest-database-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatabaseConnection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Connection name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Database type\"\n    },\n    \"connectionString\": {\n      \"type\": \"string\",\n      \"description\": \"Database connection string\"\n    },\n    \"credentials\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-database-connection-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: DatabaseConnection
---
