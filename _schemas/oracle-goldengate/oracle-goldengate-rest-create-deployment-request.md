---
description: ''
layout: schema
name: CreateDeploymentRequest
properties_list:
- description: Oracle GoldenGate home directory path
  name: oggHome
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: environmentVariables
  type: object
- description: Whether to automatically start the deployment
  name: autoStart
  type: boolean
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-create-deployment-request-schema.json
slug: oracle-goldengate-rest-create-deployment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateDeploymentRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"oggHome\": {\n      \"type\": \"string\",\n      \"description\": \"Oracle GoldenGate home directory path\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"environmentVariables\": {\n      \"type\": \"object\"\n    },\n    \"autoStart\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to automatically start the deployment\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-create-deployment-request-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: CreateDeploymentRequest
---
