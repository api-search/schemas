---
description: Scan and planning tasks for server-side scan planning - `plan-tasks` contains opaque units of planning work - `file-scan-tasks` contains a partial or complete list of table scan tasks - `delete-files` contains delete files referenced by file scan tasks Each plan task must be passed to the fetchScanTasks endpoint to fetch the file scan tasks for the plan task. The list of delete files must contain all delete files referenced by the file scan tasks.
layout: schema
name: ScanTasks
properties_list:
- description: Delete files referenced by file scan tasks
  name: delete-files
  type: array
- description: ''
  name: file-scan-tasks
  type: array
- description: ''
  name: plan-tasks
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-scan-tasks-schema.json
slug: rest-catalog-open-api-scan-tasks
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ScanTasks
---
