---
description: Paginated list of jobs.
layout: schema
name: JobList
properties_list:
- description: Pagination offset (1-based).
  name: offset
  type: integer
- description: Maximum results requested.
  name: len
  type: integer
- description: Total number of matching jobs.
  name: total
  type: integer
- description: List of workflow job entries.
  name: workflows
  type: array
- description: List of coordinator job entries.
  name: coordinatorjobs
  type: array
- description: List of bundle job entries.
  name: bundlejobs
  type: array
provider_name: Apache Oozie
provider_slug: apache-oozie
schema_file: json-schema/apache-oozie-job-list-schema.json
slug: apache-oozie-job-list
tags:
- Workflow
- Hadoop
- Orchestration
- Scheduling
- Big Data
- Apache
- Java
- Open Source
title: JobList
---
