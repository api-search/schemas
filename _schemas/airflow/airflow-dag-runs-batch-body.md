---
description: List DAG Runs body for batch endpoint.
layout: schema
name: DAGRunsBatchBody
properties_list:
- description: ''
  name: order_by
  type: object
- description: ''
  name: page_offset
  type: integer
- description: ''
  name: page_limit
  type: integer
- description: ''
  name: dag_ids
  type: object
- description: ''
  name: states
  type: object
- description: ''
  name: run_after_gte
  type: object
- description: ''
  name: run_after_gt
  type: object
- description: ''
  name: run_after_lte
  type: object
- description: ''
  name: run_after_lt
  type: object
- description: ''
  name: logical_date_gte
  type: object
- description: ''
  name: logical_date_gt
  type: object
- description: ''
  name: logical_date_lte
  type: object
- description: ''
  name: logical_date_lt
  type: object
- description: ''
  name: start_date_gte
  type: object
- description: ''
  name: start_date_gt
  type: object
- description: ''
  name: start_date_lte
  type: object
- description: ''
  name: start_date_lt
  type: object
- description: ''
  name: end_date_gte
  type: object
- description: ''
  name: end_date_gt
  type: object
- description: ''
  name: end_date_lte
  type: object
- description: ''
  name: end_date_lt
  type: object
- description: ''
  name: duration_gte
  type: object
- description: ''
  name: duration_gt
  type: object
- description: ''
  name: duration_lte
  type: object
- description: ''
  name: duration_lt
  type: object
- description: ''
  name: conf_contains
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-runs-batch-body-schema.json
slug: airflow-dag-runs-batch-body
source_filename: airflow-dag-runs-batch-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-runs-batch-body-schema.json\",\n  \"title\": \"DAGRunsBatchBody\",\n  \"description\": \"List DAG Runs body for batch endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"order_by\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Order By\"\n    },\n    \"page_offset\": {\n      \"type\": \"integer\",\n      \"minimum\": 0.0,\n      \"title\": \"Page Offset\",\n      \"default\": 0\n    },\n    \"page_limit\": {\n      \"type\": \"integer\",\n      \"minimum\": 0.0,\n      \"title\": \"Page Limit\",\n      \"default\": 100\n    },\n    \"dag_ids\": {\n      \"anyOf\": [\n        {\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"\
  array\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Ids\"\n    },\n    \"states\": {\n      \"anyOf\": [\n        {\n          \"items\": {\n            \"anyOf\": [\n              {\n                \"$ref\": \"#/components/schemas/DagRunState\"\n              },\n              {\n                \"type\": \"null\"\n              }\n            ]\n          },\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"States\"\n    },\n    \"run_after_gte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Run After Gte\"\n    },\n    \"run_after_gt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n   \
  \   ],\n      \"title\": \"Run After Gt\"\n    },\n    \"run_after_lte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Run After Lte\"\n    },\n    \"run_after_lt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Run After Lt\"\n    },\n    \"logical_date_gte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date Gte\"\n    },\n    \"logical_date_gt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"\
  title\": \"Logical Date Gt\"\n    },\n    \"logical_date_lte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date Lte\"\n    },\n    \"logical_date_lt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date Lt\"\n    },\n    \"start_date_gte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Start Date Gte\"\n    },\n    \"start_date_gt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\"\
  : \"Start Date Gt\"\n    },\n    \"start_date_lte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Start Date Lte\"\n    },\n    \"start_date_lt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Start Date Lt\"\n    },\n    \"end_date_gte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date Gte\"\n    },\n    \"end_date_gt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date Gt\"\n  \
  \  },\n    \"end_date_lte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date Lte\"\n    },\n    \"end_date_lt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date Lt\"\n    },\n    \"duration_gte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Duration Gte\"\n    },\n    \"duration_gt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Duration Gt\"\n    },\n    \"duration_lte\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n\
  \        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Duration Lte\"\n    },\n    \"duration_lt\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Duration Lt\"\n    },\n    \"conf_contains\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Conf Contains\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-runs-batch-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGRunsBatchBody
---
