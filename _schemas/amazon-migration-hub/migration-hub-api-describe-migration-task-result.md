---
description: DescribeMigrationTaskResult schema from Amazon Migration Hub API
layout: schema
name: DescribeMigrationTaskResult
properties_list:
- description: ''
  name: MigrationTask
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-describe-migration-task-result-schema.json
slug: migration-hub-api-describe-migration-task-result
source_filename: migration-hub-api-describe-migration-task-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-describe-migration-task-result-schema.json\",\n  \"title\": \"DescribeMigrationTaskResult\",\n  \"description\": \"DescribeMigrationTaskResult schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MigrationTask\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTask\"\n        },\n        {\n          \"description\": \"Object encapsulating information about the migration task.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-describe-migration-task-result-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeMigrationTaskResult
---
