---
description: enum that describes the different types of jobs that the platform runs.
layout: schema
name: JobType
properties_list: []
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-job-type-schema.json
slug: airbyte-job-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-job-type-schema.json\",\n  \"title\": \"JobType\",\n  \"description\": \"enum that describes the different types of jobs that the platform runs.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"get_spec\",\n    \"check_connection\",\n    \"discover_schema\",\n    \"sync\",\n    \"reset_connection\",\n    \"connection_updater\",\n    \"replicate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-job-type-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: JobType
---
