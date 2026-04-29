---
description: ''
layout: schema
name: DeploymentBackup
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: deploymentId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: sizeInBytes
  type: integer
- description: ''
  name: backupType
  type: string
- description: ''
  name: oggVersion
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-cloud-service-deployment-backup-schema.json
slug: oracle-goldengate-cloud-service-deployment-backup
source_filename: oracle-goldengate-cloud-service-deployment-backup-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentBackup\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"deploymentId\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\"\n    },\n    \"sizeInBytes\": {\n      \"type\": \"integer\"\n    },\n    \"backupType\": {\n      \"type\": \"string\"\n    },\n    \"oggVersion\": {\n      \"type\": \"string\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-cloud-service-deployment-backup-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: DeploymentBackup
---
