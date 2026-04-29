---
description: ListMigrationTasksResult schema from Amazon Migration Hub API
layout: schema
name: ListMigrationTasksResult
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MigrationTaskSummaryList
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-list-migration-tasks-result-schema.json
slug: migration-hub-api-list-migration-tasks-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-migration-tasks-result-schema.json\",\n  \"title\": \"ListMigrationTasksResult\",\n  \"description\": \"ListMigrationTasksResult schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"If there are more migration tasks than the max result, return the next token to be passed to the next call as a bookmark of where to start from.\"\n        }\n      ]\n    },\n    \"MigrationTaskSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTaskSummaryList\"\n        },\n        {\n          \"description\": \"Lists the migration task's summary which includes:\
  \ <code>MigrationTaskName</code>, <code>ProgressPercent</code>, <code>ProgressUpdateStream</code>, <code>Status</code>, and the <code>UpdateDateTime</code> for each task.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-migration-tasks-result-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListMigrationTasksResult
---
