---
description: Serializer for AppBuilder Menu Item responses.
layout: schema
name: AppBuilderMenuItemResponse
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: href
  type: string
- description: ''
  name: category
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-app-builder-menu-item-response-schema.json
slug: airflow-app-builder-menu-item-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-app-builder-menu-item-response-schema.json\",\n  \"title\": \"AppBuilderMenuItemResponse\",\n  \"description\": \"Serializer for AppBuilder Menu Item responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"title\": \"Href\"\n    },\n    \"category\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Category\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"href\"\n  ],\n  \"additionalProperties\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-app-builder-menu-item-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: AppBuilderMenuItemResponse
---
