---
description: Serializer for AppBuilder View responses.
layout: schema
name: AppBuilderViewResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: category
  type: object
- description: ''
  name: view
  type: object
- description: ''
  name: label
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-app-builder-view-response-schema.json
slug: airflow-app-builder-view-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-app-builder-view-response-schema.json\",\n  \"title\": \"AppBuilderViewResponse\",\n  \"description\": \"Serializer for AppBuilder View responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Name\"\n    },\n    \"category\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Category\"\n    },\n    \"view\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"View\"\n    },\n    \"label\": {\n      \"anyOf\": [\n  \
  \      {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Label\"\n    }\n  },\n  \"additionalProperties\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-app-builder-view-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: AppBuilderViewResponse
---
