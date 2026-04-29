---
description: XCom entry collection item. The value field is only available when reading a single object due to the size of the value.
layout: schema
name: XComCollectionItem
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: execution_date
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: task_id
  type: string
- description: ''
  name: timestamp
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-x-com-collection-item-schema.json
slug: openapi.yaml-x-com-collection-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-x-com-collection-item-schema.json\",\n  \"title\": \"XComCollectionItem\",\n  \"description\": \"XCom entry collection item.\\n\\nThe value field is only available when reading a single object due to the size of the value.\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"type\": \"string\"\n    },\n    \"execution_date\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"task_id\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-x-com-collection-item-schema.json
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
title: XComCollectionItem
---
