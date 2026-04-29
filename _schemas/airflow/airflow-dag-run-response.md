---
description: DAG Run serializer for responses.
layout: schema
name: DAGRunResponse
properties_list:
- description: ''
  name: dag_run_id
  type: string
- description: ''
  name: dag_id
  type: string
- description: ''
  name: logical_date
  type: object
- description: ''
  name: queued_at
  type: object
- description: ''
  name: start_date
  type: object
- description: ''
  name: end_date
  type: object
- description: ''
  name: duration
  type: object
- description: ''
  name: data_interval_start
  type: object
- description: ''
  name: data_interval_end
  type: object
- description: ''
  name: run_after
  type: string
- description: ''
  name: last_scheduling_decision
  type: object
- description: ''
  name: run_type
  type: object
- description: ''
  name: state
  type: object
- description: ''
  name: triggered_by
  type: object
- description: ''
  name: triggering_user_name
  type: object
- description: ''
  name: conf
  type: object
- description: ''
  name: note
  type: object
- description: ''
  name: dag_versions
  type: array
- description: ''
  name: bundle_version
  type: object
- description: ''
  name: dag_display_name
  type: string
- description: ''
  name: partition_key
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-run-response-schema.json
slug: airflow-dag-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-response-schema.json\",\n  \"title\": \"DAGRunResponse\",\n  \"description\": \"DAG Run serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_run_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Run Id\"\n    },\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"logical_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date\"\n    },\n    \"queued_at\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Queued\
  \ At\"\n    },\n    \"start_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Start Date\"\n    },\n    \"end_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date\"\n    },\n    \"duration\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Duration\"\n    },\n    \"data_interval_start\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Data Interval Start\"\n    },\n    \"data_interval_end\": {\n      \"anyOf\": [\n     \
  \   {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Data Interval End\"\n    },\n    \"run_after\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Run After\"\n    },\n    \"last_scheduling_decision\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Last Scheduling Decision\"\n    },\n    \"run_type\": {\n      \"$ref\": \"#/components/schemas/DagRunType\"\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/DagRunState\"\n    },\n    \"triggered_by\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DagRunTriggeredByType\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    },\n    \"triggering_user_name\": {\n      \"\
  anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Triggering User Name\"\n    },\n    \"conf\": {\n      \"anyOf\": [\n        {\n          \"additionalProperties\": true,\n          \"type\": \"object\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Conf\"\n    },\n    \"note\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Note\"\n    },\n    \"dag_versions\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DagVersionResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Dag Versions\"\n    },\n    \"bundle_version\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Bundle Version\"\n    },\n\
  \    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    },\n    \"partition_key\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Partition Key\"\n    }\n  },\n  \"required\": [\n    \"dag_run_id\",\n    \"dag_id\",\n    \"logical_date\",\n    \"queued_at\",\n    \"start_date\",\n    \"end_date\",\n    \"duration\",\n    \"data_interval_start\",\n    \"data_interval_end\",\n    \"run_after\",\n    \"last_scheduling_decision\",\n    \"run_type\",\n    \"state\",\n    \"triggered_by\",\n    \"triggering_user_name\",\n    \"conf\",\n    \"note\",\n    \"dag_versions\",\n    \"bundle_version\",\n    \"dag_display_name\",\n    \"partition_key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGRunResponse
---
