---
description: In response to a request by the <code>DescribeReplicationTasks</code> operation, this object provides a collection of statistics about a replication task.
layout: schema
name: ReplicationTaskStats
properties_list:
- description: ''
  name: FullLoadProgressPercent
  type: object
- description: ''
  name: ElapsedTimeMillis
  type: object
- description: ''
  name: TablesLoaded
  type: object
- description: ''
  name: TablesLoading
  type: object
- description: ''
  name: TablesQueued
  type: object
- description: ''
  name: TablesErrored
  type: object
- description: ''
  name: FreshStartDate
  type: object
- description: ''
  name: StartDate
  type: object
- description: ''
  name: StopDate
  type: object
- description: ''
  name: FullLoadStartDate
  type: object
- description: ''
  name: FullLoadFinishDate
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-replication-task-stats-schema.json
slug: amazon-dms-replication-task-stats
source_filename: amazon-dms-replication-task-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-task-stats-schema.json\",\n  \"title\": \"ReplicationTaskStats\",\n  \"description\": \"In response to a request by the <code>DescribeReplicationTasks</code> operation, this object provides a collection of statistics about a replication task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FullLoadProgressPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The percent complete for the full load migration task.\"\n        }\n      ]\n    },\n    \"ElapsedTimeMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The elapsed time of the task, in milliseconds.\"\n        }\n      ]\n    },\n\
  \    \"TablesLoaded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of tables loaded for this task.\"\n        }\n      ]\n    },\n    \"TablesLoading\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of tables currently loading for this task.\"\n        }\n      ]\n    },\n    \"TablesQueued\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of tables queued for this task.\"\n        }\n      ]\n    },\n    \"TablesErrored\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of errors that have occurred during this task.\"\n        }\n      ]\n    },\n    \"FreshStartDate\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the replication task was started either with a fresh start or a target reload.\"\n        }\n      ]\n    },\n    \"StartDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the replication task was started either with a fresh start or a resume. For more information, see <a href=\\\"https://docs.aws.amazon.com/dms/latest/APIReference/API_StartReplicationTask.html#DMS-StartReplicationTask-request-StartReplicationTaskType\\\">StartReplicationTaskType</a>.\"\n        }\n      ]\n    },\n    \"StopDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the replication task was stopped.\"\n        }\n      ]\n    },\n    \"FullLoadStartDate\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the replication task full load was started.\"\n        }\n      ]\n    },\n    \"FullLoadFinishDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the replication task full load was completed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-task-stats-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: ReplicationTaskStats
---
