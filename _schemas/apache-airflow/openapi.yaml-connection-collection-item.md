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
