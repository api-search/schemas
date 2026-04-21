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
