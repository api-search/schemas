---
description: Trigger DAG Run Serializer for POST body.
layout: schema
name: TriggerDAGRunPostBody
properties_list:
- description: ''
  name: dag_run_id
  type: object
- description: ''
  name: data_interval_start
  type: object
- description: ''
  name: data_interval_end
  type: object
- description: ''
  name: logical_date
  type: object
- description: ''
  name: run_after
  type: object
- description: ''
  name: conf
  type: object
- description: ''
  name: note
  type: object
- description: ''
  name: partition_key
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-trigger-dag-run-post-body-schema.json
slug: airflow-trigger-dag-run-post-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-trigger-dag-run-post-body-schema.json\",\n  \"title\": \"TriggerDAGRunPostBody\",\n  \"description\": \"Trigger DAG Run Serializer for POST body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_run_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Run Id\"\n    },\n    \"data_interval_start\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Data Interval Start\"\n    },\n    \"data_interval_end\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n    \
  \      \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Data Interval End\"\n    },\n    \"logical_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date\"\n    },\n    \"run_after\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Run After\"\n    },\n    \"conf\": {\n      \"anyOf\": [\n        {\n          \"additionalProperties\": true,\n          \"type\": \"object\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Conf\"\n    },\n    \"note\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Note\"\n    },\n  \
  \  \"partition_key\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Partition Key\"\n    }\n  },\n  \"required\": [\n    \"logical_date\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-trigger-dag-run-post-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TriggerDAGRunPostBody
---
