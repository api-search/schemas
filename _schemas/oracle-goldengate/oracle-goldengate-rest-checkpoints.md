---
description: ''
layout: schema
name: Checkpoints
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: readCheckpoint
  type: object
- description: ''
  name: writeCheckpoint
  type: object
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-checkpoints-schema.json
slug: oracle-goldengate-rest-checkpoints
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Checkpoints\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"readCheckpoint\": {\n      \"type\": \"object\"\n    },\n    \"writeCheckpoint\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-checkpoints-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Checkpoints
---
