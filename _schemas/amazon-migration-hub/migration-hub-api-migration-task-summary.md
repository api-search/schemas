---
description: MigrationTaskSummary includes <code>MigrationTaskName</code>, <code>ProgressPercent</code>, <code>ProgressUpdateStream</code>, <code>Status</code>, and <code>UpdateDateTime</code> for each task.
layout: schema
name: MigrationTaskSummary
properties_list:
- description: ''
  name: ProgressUpdateStream
  type: object
- description: ''
  name: MigrationTaskName
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: ProgressPercent
  type: object
- description: ''
  name: StatusDetail
  type: object
- description: ''
  name: UpdateDateTime
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-migration-task-summary-schema.json
slug: migration-hub-api-migration-task-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-migration-task-summary-schema.json\",\n  \"title\": \"MigrationTaskSummary\",\n  \"description\": \"MigrationTaskSummary includes <code>MigrationTaskName</code>, <code>ProgressPercent</code>, <code>ProgressUpdateStream</code>, <code>Status</code>, and <code>UpdateDateTime</code> for each task.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"An AWS resource used for access control. It should uniquely identify the migration tool as it is used for all updates made by the tool.\"\n        }\n      ]\n    },\n    \"MigrationTaskName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTaskName\"\
  \n        },\n        {\n          \"description\": \"Unique identifier that references the migration task. <i>Do not store personal data in this field.</i> \"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"Status of the task.\"\n        }\n      ]\n    },\n    \"ProgressPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressPercent\"\n        },\n        {\n          \"description\": \"Indication of the percentage completion of the task.\"\n        }\n      ]\n    },\n    \"StatusDetail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusDetail\"\n        },\n        {\n          \"description\": \"Detail information of what is being done within the overall status state.\"\n        }\n      ]\n    },\n    \"UpdateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/UpdateDateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the task was gathered.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-migration-task-summary-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MigrationTaskSummary
---
