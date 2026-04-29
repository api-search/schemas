---
description: Serializer for External View Plugin responses.
layout: schema
name: ExternalViewResponse
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: icon
  type: object
- description: ''
  name: icon_dark_mode
  type: object
- description: ''
  name: url_route
  type: object
- description: ''
  name: category
  type: object
- description: ''
  name: href
  type: string
- description: ''
  name: destination
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-external-view-response-schema.json
slug: airflow-external-view-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-external-view-response-schema.json\",\n  \"title\": \"ExternalViewResponse\",\n  \"description\": \"Serializer for External View Plugin responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"icon\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Icon\"\n    },\n    \"icon_dark_mode\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Icon Dark Mode\"\n    },\n    \"url_route\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n\
  \        }\n      ],\n      \"title\": \"Url Route\"\n    },\n    \"category\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Category\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"title\": \"Href\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"nav\",\n        \"dag\",\n        \"dag_run\",\n        \"task\",\n        \"task_instance\",\n        \"base\"\n      ],\n      \"title\": \"Destination\",\n      \"default\": \"nav\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"href\"\n  ],\n  \"additionalProperties\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-external-view-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ExternalViewResponse
---
