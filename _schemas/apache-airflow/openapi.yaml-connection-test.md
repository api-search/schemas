---
description: Connection test results. *New in version 2.2.0*
layout: schema
name: ConnectionTest
properties_list:
- description: The success or failure message of the request.
  name: message
  type: string
- description: The status of the request.
  name: status
  type: boolean
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-connection-test-schema.json
slug: openapi.yaml-connection-test
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-connection-test-schema.json\",\n  \"title\": \"ConnectionTest\",\n  \"description\": \"Connection test results.\\n\\n*New in version 2.2.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"description\": \"The success or failure message of the request.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the request.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-connection-test-schema.json
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
title: ConnectionTest
---
