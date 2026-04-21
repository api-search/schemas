---
description: ImportError schema from Apache Airflow API
layout: schema
name: ImportError
properties_list:
- description: The filename
  name: filename
  type: string
- description: The import error ID.
  name: import_error_id
  type: integer
- description: The full stackstrace..
  name: stack_trace
  type: string
- description: The time when this error was created.
  name: timestamp
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-import-error-schema.json
slug: openapi.yaml-import-error
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
title: ImportError
---
