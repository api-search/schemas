---
description: Task state. *Changed in version 2.0.2*&#58; 'removed' is added as a possible value. *Changed in version 2.2.0*&#58; 'deferred' is added as a possible value. *Changed in version 2.4.0*&#58; 'sensing' state has been removed. *Changed in version 2.4.2*&#58; 'restarting' is added as a possible value
layout: schema
name: TaskState
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-state-schema.json
slug: openapi.yaml-task-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-state-schema.json\",\n  \"title\": \"TaskState\",\n  \"description\": \"Task state.\\n\\n*Changed in version 2.0.2*&#58; 'removed' is added as a possible value.\\n\\n*Changed in version 2.2.0*&#58; 'deferred' is added as a possible value.\\n\\n*Changed in version 2.4.0*&#58; 'sensing' state has been removed.\\n*Changed in version 2.4.2*&#58; 'restarting' is added as a possible value\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"success\",\n    \"running\",\n    \"failed\",\n    \"upstream_failed\",\n    \"skipped\",\n    \"up_for_retry\",\n    \"up_for_reschedule\",\n    \"queued\",\n    \"none\",\n    \"scheduled\",\n    \"deferred\",\n    \"removed\",\n    \"restarting\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-state-schema.json
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
title: TaskState
---
