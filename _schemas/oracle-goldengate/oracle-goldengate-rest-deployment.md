---
description: ''
layout: schema
name: Deployment
properties_list:
- description: Unique name of the deployment
  name: name
  type: string
- description: Current status of the deployment
  name: status
  type: string
- description: Description of the deployment
  name: description
  type: string
- description: Oracle GoldenGate home directory
  name: oggHome
  type: string
- description: GoldenGate software version
  name: oggVersion
  type: string
- description: ''
  name: environmentVariables
  type: object
- description: ''
  name: services
  type: array
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-deployment-schema.json
slug: oracle-goldengate-rest-deployment
source_filename: oracle-goldengate-rest-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the deployment\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the deployment\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the deployment\"\n    },\n    \"oggHome\": {\n      \"type\": \"string\",\n      \"description\": \"Oracle GoldenGate home directory\"\n    },\n    \"oggVersion\": {\n      \"type\": \"string\",\n      \"description\": \"GoldenGate software version\"\n    },\n    \"environmentVariables\": {\n      \"type\": \"object\"\n    },\n    \"services\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-deployment-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Deployment
---
