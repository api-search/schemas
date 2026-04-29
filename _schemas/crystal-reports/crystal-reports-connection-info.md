---
description: Database connection information for the report instance
layout: schema
name: ConnectionInfo
properties_list:
- description: Database username
  name: userName
  type: string
- description: Database password
  name: password
  type: string
- description: Database server name or address
  name: serverName
  type: string
- description: Database name
  name: databaseName
  type: string
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-connection-info-schema.json
slug: crystal-reports-connection-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-connection-info-schema.json\",\n  \"title\": \"ConnectionInfo\",\n  \"description\": \"Database connection information for the report instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Database username\",\n      \"example\": \"db_user\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Database password\",\n      \"example\": \"db_pass\"\n    },\n    \"serverName\": {\n      \"type\": \"string\",\n      \"description\": \"Database server name or address\",\n      \"example\": \"dbserver.example.com\"\n    },\n    \"databaseName\": {\n      \"type\": \"string\",\n      \"description\": \"Database name\",\n      \"example\": \"SalesDB\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-connection-info-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: ConnectionInfo
---
