---
description: The pool
layout: schema
name: Pool
properties_list:
- description: The description of the pool. *New in version 2.3.0*
  name: description
  type: string
- description: The name of pool.
  name: name
  type: string
- description: The number of slots used by running/queued tasks at the moment.
  name: occupied_slots
  type: integer
- description: The number of free slots at the moment.
  name: open_slots
  type: integer
- description: The number of slots used by queued tasks at the moment.
  name: queued_slots
  type: integer
- description: The maximum number of slots that can be assigned to tasks. One job may occupy one or more slots.
  name: slots
  type: integer
- description: The number of slots used by running tasks at the moment.
  name: used_slots
  type: integer
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-pool-schema.json
slug: openapi.yaml-pool
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
title: Pool
---
