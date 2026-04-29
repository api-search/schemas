---
description: ''
layout: schema
name: DatabaseRegistration
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: databaseId
  type: string
- description: ''
  name: connectionString
  type: string
- description: ''
  name: username
  type: string
- description: ''
  name: fqdn
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-cloud-service-database-registration-schema.json
slug: oracle-goldengate-cloud-service-database-registration
source_filename: oracle-goldengate-cloud-service-database-registration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatabaseRegistration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\"\n    },\n    \"databaseId\": {\n      \"type\": \"string\"\n    },\n    \"connectionString\": {\n      \"type\": \"string\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-cloud-service-database-registration-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: DatabaseRegistration
---
