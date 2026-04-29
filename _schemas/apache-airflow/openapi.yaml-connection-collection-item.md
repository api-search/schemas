---
description: Connection collection item. The password and extra fields are only available when retrieving a single object due to the sensitivity of this data.
layout: schema
name: ConnectionCollectionItem
properties_list:
- description: The connection type.
  name: conn_type
  type: string
- description: The connection ID.
  name: connection_id
  type: string
- description: The description of the connection.
  name: description
  type: string
- description: Host of the connection.
  name: host
  type: string
- description: Login of the connection.
  name: login
  type: string
- description: Port of the connection.
  name: port
  type: integer
- description: Schema of the connection.
  name: schema
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-connection-collection-item-schema.json
slug: openapi.yaml-connection-collection-item
source_filename: openapi.yaml-connection-collection-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-connection-collection-item-schema.json\",\n  \"title\": \"ConnectionCollectionItem\",\n  \"description\": \"Connection collection item.\\nThe password and extra fields are only available when retrieving a single object due to the sensitivity of this data.\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conn_type\": {\n      \"description\": \"The connection type.\",\n      \"type\": \"string\"\n    },\n    \"connection_id\": {\n      \"description\": \"The connection ID.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"The description of the connection.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"host\": {\n      \"description\": \"Host of the connection.\",\n      \"nullable\": true,\n      \"type\": \"string\"\
  \n    },\n    \"login\": {\n      \"description\": \"Login of the connection.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"port\": {\n      \"description\": \"Port of the connection.\",\n      \"nullable\": true,\n      \"type\": \"integer\"\n    },\n    \"schema\": {\n      \"description\": \"Schema of the connection.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-connection-collection-item-schema.json
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
title: ConnectionCollectionItem
---
