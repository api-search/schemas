---
description: A single action within a workflow job.
layout: schema
name: JobAction
properties_list:
- description: Action identifier.
  name: id
  type: string
- description: Action name as defined in the workflow.
  name: name
  type: string
- description: Action type (map-reduce, pig, hive, etc.).
  name: type
  type: string
- description: Current action status.
  name: status
  type: string
- description: Action start timestamp.
  name: startTime
  type: string
- description: Action end timestamp.
  name: endTime
  type: string
- description: Error code if the action failed.
  name: errorCode
  type: string
- description: Error message if the action failed.
  name: errorMessage
  type: string
provider_name: Apache Oozie
provider_slug: apache-oozie
schema_file: json-schema/apache-oozie-job-action-schema.json
slug: apache-oozie-job-action
source_filename: apache-oozie-job-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-job-action-schema.json\",\n  \"title\": \"JobAction\",\n  \"description\": \"A single action within a workflow job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Action identifier.\",\n      \"example\": \"0000001-200101120000000-oozie-admin-W@action1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Action name as defined in the workflow.\",\n      \"example\": \"my-map-reduce\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Action type (map-reduce, pig, hive, etc.).\",\n      \"example\": \"map-reduce\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current action status.\",\n      \"example\": \"OK\"\n    },\n    \"startTime\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Action start timestamp.\",\n      \"example\": \"2021-01-01T12:00:00.000Z\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Action end timestamp.\",\n      \"example\": \"2021-01-01T12:05:00.000Z\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Error code if the action failed.\",\n      \"example\": null\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the action failed.\",\n      \"example\": null\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/json-schema/apache-oozie-job-action-schema.json
tags:
- Workflow
- Hadoop
- Orchestration
- Scheduling
- Big Data
- Apache
- Java
- Open Source
title: JobAction
---
