---
description: Contains metadata for a replication instance task log.
layout: schema
name: ReplicationInstanceTaskLog
properties_list:
- description: ''
  name: ReplicationTaskName
  type: object
- description: ''
  name: ReplicationTaskArn
  type: object
- description: ''
  name: ReplicationInstanceTaskLogSize
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-replication-instance-task-log-schema.json
slug: amazon-dms-replication-instance-task-log
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-instance-task-log-schema.json\",\n  \"title\": \"ReplicationInstanceTaskLog\",\n  \"description\": \"Contains metadata for a replication instance task log.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReplicationTaskName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the replication task.\"\n        }\n      ]\n    },\n    \"ReplicationTaskArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication task.\"\n        }\n      ]\n    },\n    \"ReplicationInstanceTaskLogSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\
  \n        },\n        {\n          \"description\": \"The size, in bytes, of the replication task log.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-instance-task-log-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: ReplicationInstanceTaskLog
---
