---
description: Task object encapsulating task information.
layout: schema
name: Task
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusDetail
  type: object
- description: ''
  name: ProgressPercent
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-task-schema.json
slug: migration-hub-api-task
source_filename: migration-hub-api-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"Task object encapsulating task information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"description\": \"Status of the task - Not Started, In-Progress, Complete.\"\n        }\n      ]\n    },\n    \"StatusDetail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusDetail\"\n        },\n        {\n          \"description\": \"Details of task status as notified by a migration tool. A tool might use this field to provide clarifying information about the status that is unique to that tool or that explains an error state.\"\n        }\n      ]\n\
  \    },\n    \"ProgressPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressPercent\"\n        },\n        {\n          \"description\": \"Indication of the percentage completion of the task.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-task-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Task
---
