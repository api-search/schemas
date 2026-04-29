---
description: Schedule interval. Defines how often DAG runs, this object gets added to your latest task instance's execution_date to figure out the next schedule.
layout: schema
name: ScheduleInterval
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-schedule-interval-schema.json
slug: openapi.yaml-schedule-interval
source_filename: openapi.yaml-schedule-interval-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-schedule-interval-schema.json\",\n  \"title\": \"ScheduleInterval\",\n  \"description\": \"Schedule interval. Defines how often DAG runs, this object gets added to your latest task instance's\\nexecution_date to figure out the next schedule.\\n\",\n  \"anyOf\": [\n    {\n      \"$ref\": \"#/components/schemas/TimeDelta\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RelativeDelta\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/CronExpression\"\n    }\n  ],\n  \"readOnly\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-schedule-interval-schema.json
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
title: ScheduleInterval
---
