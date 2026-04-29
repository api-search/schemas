---
description: The Action-Resource item. *New in version 2.1.0*
layout: schema
name: ActionResource
properties_list:
- description: The permission action
  name: action
  type: object
- description: The permission resource
  name: resource
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-action-resource-schema.json
slug: openapi.yaml-action-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-action-resource-schema.json\",\n  \"title\": \"ActionResource\",\n  \"description\": \"The Action-Resource item.\\n\\n*New in version 2.1.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"$ref\": \"#/components/schemas/Action\",\n      \"description\": \"The permission action\",\n      \"type\": \"object\"\n    },\n    \"resource\": {\n      \"$ref\": \"#/components/schemas/Resource\",\n      \"description\": \"The permission resource\",\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-action-resource-schema.json
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
title: ActionResource
---
