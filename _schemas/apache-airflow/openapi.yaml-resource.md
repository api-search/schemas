---
description: A resource on which permissions are granted. *New in version 2.1.0*
layout: schema
name: Resource
properties_list:
- description: The name of the resource
  name: name
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-resource-schema.json
slug: openapi.yaml-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"description\": \"A resource on which permissions are granted.\\n\\n*New in version 2.1.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The name of the resource\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-resource-schema.json
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
title: Resource
---
