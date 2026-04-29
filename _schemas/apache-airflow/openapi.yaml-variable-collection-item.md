---
description: XCom entry collection item. The value field are only available when retrieving a single object due to the sensitivity of this data.
layout: schema
name: VariableCollectionItem
properties_list:
- description: The description of the variable. *New in version 2.4.0*
  name: description
  type: string
- description: ''
  name: key
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-variable-collection-item-schema.json
slug: openapi.yaml-variable-collection-item
source_filename: openapi.yaml-variable-collection-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-variable-collection-item-schema.json\",\n  \"title\": \"VariableCollectionItem\",\n  \"description\": \"XCom entry collection item.\\nThe value field are only available when retrieving a single object due to the sensitivity of this data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description of the variable.\\n\\n*New in version 2.4.0*\\n\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-variable-collection-item-schema.json
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
title: VariableCollectionItem
---
