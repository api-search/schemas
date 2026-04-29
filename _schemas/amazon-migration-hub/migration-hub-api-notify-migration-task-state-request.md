---
description: NotifyMigrationTaskStateRequest schema from Amazon Migration Hub API
layout: schema
name: NotifyMigrationTaskStateRequest
properties_list:
- description: ''
  name: ProgressUpdateStream
  type: object
- description: ''
  name: MigrationTaskName
  type: object
- description: ''
  name: Task
  type: object
- description: ''
  name: UpdateDateTime
  type: object
- description: ''
  name: NextUpdateSeconds
  type: object
- description: ''
  name: DryRun
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-notify-migration-task-state-request-schema.json
slug: migration-hub-api-notify-migration-task-state-request
source_filename: migration-hub-api-notify-migration-task-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-notify-migration-task-state-request-schema.json\",\n  \"title\": \"NotifyMigrationTaskStateRequest\",\n  \"description\": \"NotifyMigrationTaskStateRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"The name of the ProgressUpdateStream. \"\n        }\n      ]\n    },\n    \"MigrationTaskName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTaskName\"\n        },\n        {\n          \"description\": \"Unique identifier that references the migration task. <i>Do not store personal data in this field.</i> \"\n        }\n\
  \      ]\n    },\n    \"Task\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Task\"\n        },\n        {\n          \"description\": \"Information about the task's progress and status.\"\n        }\n      ]\n    },\n    \"UpdateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the task was gathered.\"\n        }\n      ]\n    },\n    \"NextUpdateSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextUpdateSeconds\"\n        },\n        {\n          \"description\": \"Number of seconds after the UpdateDateTime within which the Migration Hub can expect an update. If Migration Hub does not receive an update within the specified interval, then the migration task will be considered stale.\"\n        }\n      ]\n    },\n    \"DryRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DryRun\"\
  \n        },\n        {\n          \"description\": \"Optional boolean flag to indicate whether any effect should take place. Used to test if the caller has permission to make the call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ProgressUpdateStream\",\n    \"MigrationTaskName\",\n    \"Task\",\n    \"UpdateDateTime\",\n    \"NextUpdateSeconds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-notify-migration-task-state-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NotifyMigrationTaskStateRequest
---
