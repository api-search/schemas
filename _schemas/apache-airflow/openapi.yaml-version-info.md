---
description: Version information.
layout: schema
name: VersionInfo
properties_list:
- description: The git version (including git commit hash)
  name: git_version
  type: string
- description: The version of Airflow
  name: version
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-version-info-schema.json
slug: openapi.yaml-version-info
source_filename: openapi.yaml-version-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-version-info-schema.json\",\n  \"title\": \"VersionInfo\",\n  \"description\": \"Version information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"git_version\": {\n      \"description\": \"The git version (including git commit hash)\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"description\": \"The version of Airflow\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-version-info-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: VersionInfo
---
