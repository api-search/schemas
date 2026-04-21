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
