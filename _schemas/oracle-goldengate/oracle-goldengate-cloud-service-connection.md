---
description: ''
layout: schema
name: Connection
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
  name: connectionType
  type: string
- description: ''
  name: technologyType
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
- description: ''
  name: timeUpdated
  type: string
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-cloud-service-connection-schema.json
slug: oracle-goldengate-cloud-service-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Connection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\"\n    },\n    \"connectionType\": {\n      \"type\": \"string\"\n    },\n    \"technologyType\": {\n      \"type\": \"string\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\"\n    },\n    \"timeUpdated\": {\n      \"type\": \"string\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-cloud-service-connection-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Connection
---
