---
description: ''
layout: schema
name: ValidateDatabaseRequest
properties_list:
- description: ''
  name: host
  type: string
- description: ''
  name: port
  type: integer
- description: ''
  name: databaseType
  type: string
- description: ''
  name: serviceName
  type: string
- description: ''
  name: username
  type: string
- description: ''
  name: password
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-veridata-rest-validate-database-request-schema.json
slug: oracle-goldengate-veridata-rest-validate-database-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ValidateDatabaseRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\n    },\n    \"databaseType\": {\n      \"type\": \"string\"\n    },\n    \"serviceName\": {\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-veridata-rest-validate-database-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: ValidateDatabaseRequest
---
