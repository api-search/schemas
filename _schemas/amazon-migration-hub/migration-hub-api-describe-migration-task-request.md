---
description: DescribeMigrationTaskRequest schema from Amazon Migration Hub API
layout: schema
name: DescribeMigrationTaskRequest
properties_list:
- description: ''
  name: ProgressUpdateStream
  type: object
- description: ''
  name: MigrationTaskName
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-describe-migration-task-request-schema.json
slug: migration-hub-api-describe-migration-task-request
source_filename: migration-hub-api-describe-migration-task-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-describe-migration-task-request-schema.json\",\n  \"title\": \"DescribeMigrationTaskRequest\",\n  \"description\": \"DescribeMigrationTaskRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"The name of the ProgressUpdateStream. \"\n        }\n      ]\n    },\n    \"MigrationTaskName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTaskName\"\n        },\n        {\n          \"description\": \"The identifier given to the MigrationTask. <i>Do not store personal data in this field.</i> \"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"ProgressUpdateStream\",\n    \"MigrationTaskName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-describe-migration-task-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeMigrationTaskRequest
---
