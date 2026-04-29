---
description: Full information about a workflow, coordinator, or bundle job.
layout: schema
name: JobInfo
properties_list:
- description: Job identifier.
  name: id
  type: string
- description: Application name from the workflow definition.
  name: appName
  type: string
- description: HDFS path to the workflow application.
  name: appPath
  type: string
- description: Current job status.
  name: status
  type: string
- description: User who submitted the job.
  name: user
  type: string
- description: User group for the job.
  name: group
  type: string
- description: Job start timestamp.
  name: startTime
  type: string
- description: Job end timestamp (null if still running).
  name: endTime
  type: string
- description: Last modification timestamp.
  name: lastModTime
  type: string
- description: Job creation timestamp.
  name: createdTime
  type: string
- description: Run number for rerun tracking.
  name: run
  type: integer
- description: List of actions within the job (workflow jobs only).
  name: actions
  type: array
provider_name: Apache Oozie
provider_slug: apache-oozie
schema_file: json-schema/apache-oozie-job-info-schema.json
slug: apache-oozie-job-info
source_filename: apache-oozie-job-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-job-info-schema.json\",\n  \"title\": \"JobInfo\",\n  \"description\": \"Full information about a workflow, coordinator, or bundle job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Job identifier.\",\n      \"example\": \"0000001-200101120000000-oozie-admin-W\"\n    },\n    \"appName\": {\n      \"type\": \"string\",\n      \"description\": \"Application name from the workflow definition.\",\n      \"example\": \"my-workflow\"\n    },\n    \"appPath\": {\n      \"type\": \"string\",\n      \"description\": \"HDFS path to the workflow application.\",\n      \"example\": \"hdfs://localhost:8020/user/admin/workflow\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current job status.\",\n\
  \      \"example\": \"RUNNING\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"User who submitted the job.\",\n      \"example\": \"admin\"\n    },\n    \"group\": {\n      \"type\": \"string\",\n      \"description\": \"User group for the job.\",\n      \"example\": \"users\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job start timestamp.\",\n      \"example\": \"2021-01-01T12:00:00.000Z\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job end timestamp (null if still running).\"\n    },\n    \"lastModTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp.\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job creation timestamp.\"\n    },\n    \"run\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Run number for rerun tracking.\",\n      \"example\": 0\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"description\": \"List of actions within the job (workflow jobs only).\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single action within a workflow job.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Action identifier.\",\n            \"example\": \"0000001-200101120000000-oozie-admin-W@action1\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Action name as defined in the workflow.\",\n            \"example\": \"my-map-reduce\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"Action type (map-reduce, pig, hive, etc.).\",\n            \"example\": \"map-reduce\"\n          },\n          \"status\": {\n        \
  \    \"type\": \"string\",\n            \"description\": \"Current action status.\",\n            \"example\": \"OK\"\n          },\n          \"startTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Action start timestamp.\",\n            \"example\": \"2021-01-01T12:00:00.000Z\"\n          },\n          \"endTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Action end timestamp.\",\n            \"example\": \"2021-01-01T12:05:00.000Z\"\n          },\n          \"errorCode\": {\n            \"type\": \"string\",\n            \"description\": \"Error code if the action failed.\",\n            \"example\": null\n          },\n          \"errorMessage\": {\n            \"type\": \"string\",\n            \"description\": \"Error message if the action failed.\",\n            \"example\": null\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-job-info-schema.json
tags:
- Workflow
- Hadoop
- Orchestration
- Scheduling
- Big Data
- Apache
- Java
- Open Source
title: JobInfo
---
