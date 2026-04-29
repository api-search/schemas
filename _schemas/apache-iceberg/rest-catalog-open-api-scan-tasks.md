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
source_filename: rest-catalog-open-api-scan-tasks-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-scan-tasks-schema.json\",\n  \"title\": \"ScanTasks\",\n  \"description\": \"Scan and planning tasks for server-side scan planning\\n\\n- `plan-tasks` contains opaque units of planning work\\n- `file-scan-tasks` contains a partial or complete list of table scan tasks\\n- `delete-files` contains delete files referenced by file scan tasks\\n\\nEach plan task must be passed to the fetchScanTasks endpoint to fetch the file scan tasks for the plan task.\\n\\nThe list of delete files must contain all delete files referenced by the file scan tasks.\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"delete-files\": {\n      \"description\": \"Delete files referenced by file scan tasks\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DeleteFile\"\
  \n      }\n    },\n    \"file-scan-tasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FileScanTask\"\n      }\n    },\n    \"plan-tasks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PlanTask\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-scan-tasks-schema.json
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
