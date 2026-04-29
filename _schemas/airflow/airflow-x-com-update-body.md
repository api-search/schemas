---
description: Payload serializer for updating an XCom entry.
layout: schema
name: XComUpdateBody
properties_list:
- description: ''
  name: value
  type: object
- description: ''
  name: map_index
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-x-com-update-body-schema.json
slug: airflow-x-com-update-body
source_filename: airflow-x-com-update-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-x-com-update-body-schema.json\",\n  \"title\": \"XComUpdateBody\",\n  \"description\": \"Payload serializer for updating an XCom entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"title\": \"Value\"\n    },\n    \"map_index\": {\n      \"type\": \"integer\",\n      \"title\": \"Map Index\",\n      \"default\": -1\n    }\n  },\n  \"required\": [\n    \"value\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-x-com-update-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: XComUpdateBody
---
