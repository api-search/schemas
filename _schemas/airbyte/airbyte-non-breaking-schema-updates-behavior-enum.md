---
description: Set how Airbyte handles syncs when it detects a non-breaking schema change in the source
layout: schema
name: NonBreakingSchemaUpdatesBehaviorEnum
properties_list: []
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-non-breaking-schema-updates-behavior-enum-schema.json
slug: airbyte-non-breaking-schema-updates-behavior-enum
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-non-breaking-schema-updates-behavior-enum-schema.json\",\n  \"title\": \"NonBreakingSchemaUpdatesBehaviorEnum\",\n  \"description\": \"Set how Airbyte handles syncs when it detects a non-breaking schema change in the source\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ignore\",\n    \"disable_connection\",\n    \"propagate_columns\",\n    \"propagate_fully\"\n  ],\n  \"default\": \"ignore\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-non-breaking-schema-updates-behavior-enum-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: NonBreakingSchemaUpdatesBehaviorEnum
---
