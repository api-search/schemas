---
description: Version information serializer for responses.
layout: schema
name: VersionInfo
properties_list:
- description: ''
  name: version
  type: string
- description: ''
  name: git_version
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-version-info-schema.json
slug: airflow-version-info
source_filename: airflow-version-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-version-info-schema.json\",\n  \"title\": \"VersionInfo\",\n  \"description\": \"Version information serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"title\": \"Version\"\n    },\n    \"git_version\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Git Version\"\n    }\n  },\n  \"required\": [\n    \"version\",\n    \"git_version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-version-info-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: VersionInfo
---
