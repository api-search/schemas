---
description: SetTaskInstanceNote schema from Apache Airflow API
layout: schema
name: SetTaskInstanceNote
properties_list:
- description: The custom note to set for this Task Instance.
  name: note
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-set-task-instance-note-schema.json
slug: openapi.yaml-set-task-instance-note
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-set-task-instance-note-schema.json\",\n  \"title\": \"SetTaskInstanceNote\",\n  \"description\": \"SetTaskInstanceNote schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"note\": {\n      \"description\": \"The custom note to set for this Task Instance.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"note\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-set-task-instance-note-schema.json
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
title: SetTaskInstanceNote
---
