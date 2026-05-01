---
description: Represents a migration task in a migration tool.
layout: schema
name: MigrationTask
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
  name: ResourceAttributeList
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-migration-task-schema.json
slug: migration-hub-api-migration-task
source_filename: migration-hub-api-migration-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-migration-task-schema.json\",\n  \"title\": \"MigrationTask\",\n  \"description\": \"Represents a migration task in a migration tool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"A name that identifies the vendor of the migration tool being used.\"\n        }\n      ]\n    },\n    \"MigrationTaskName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTaskName\"\n        },\n        {\n          \"description\": \"Unique identifier that references the migration task. <i>Do not store personal data in this field.</i> \"\n        }\n      ]\n    },\n    \"Task\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Task\"\n        },\n        {\n          \"description\": \"Task object encapsulating task information.\"\n        }\n      ]\n    },\n    \"UpdateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the task was gathered.\"\n        }\n      ]\n    },\n    \"ResourceAttributeList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LatestResourceAttributeList\"\n        },\n        {\n          \"description\": \"Information about the resource that is being migrated. This data will be used to map the task to a resource in the Application Discovery Service repository.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-migration-task-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MigrationTask
---
