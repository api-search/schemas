---
description: Task serializer for responses.
layout: schema
name: TaskResponse
properties_list:
- description: ''
  name: task_id
  type: object
- description: ''
  name: task_display_name
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: start_date
  type: object
- description: ''
  name: end_date
  type: object
- description: ''
  name: trigger_rule
  type: object
- description: ''
  name: depends_on_past
  type: boolean
- description: ''
  name: wait_for_downstream
  type: boolean
- description: ''
  name: retries
  type: object
- description: ''
  name: queue
  type: object
- description: ''
  name: pool
  type: object
- description: ''
  name: pool_slots
  type: object
- description: ''
  name: execution_timeout
  type: object
- description: ''
  name: retry_delay
  type: object
- description: ''
  name: retry_exponential_backoff
  type: number
- description: ''
  name: priority_weight
  type: object
- description: ''
  name: weight_rule
  type: object
- description: ''
  name: ui_color
  type: object
- description: ''
  name: ui_fgcolor
  type: object
- description: ''
  name: template_fields
  type: object
- description: ''
  name: downstream_task_ids
  type: object
- description: ''
  name: doc_md
  type: object
- description: ''
  name: operator_name
  type: object
- description: ''
  name: params
  type: object
- description: ''
  name: class_ref
  type: object
- description: ''
  name: is_mapped
  type: object
- description: Extract and return extra_links.
  name: extra_links
  type: array
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-response-schema.json
slug: airflow-task-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-response-schema.json\",\n  \"title\": \"TaskResponse\",\n  \"description\": \"Task serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"task_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Task Id\"\n    },\n    \"task_display_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Task Display Name\"\n    },\n    \"owner\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Owner\"\n    },\n    \"start_date\": {\n      \"anyOf\": [\n    \
  \    {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Start Date\"\n    },\n    \"end_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date\"\n    },\n    \"trigger_rule\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Trigger Rule\"\n    },\n    \"depends_on_past\": {\n      \"type\": \"boolean\",\n      \"title\": \"Depends On Past\"\n    },\n    \"wait_for_downstream\": {\n      \"type\": \"boolean\",\n      \"title\": \"Wait For Downstream\"\n    },\n    \"retries\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n   \
  \   ],\n      \"title\": \"Retries\"\n    },\n    \"queue\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Queue\"\n    },\n    \"pool\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Pool\"\n    },\n    \"pool_slots\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Pool Slots\"\n    },\n    \"execution_timeout\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeDelta\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    },\n    \"retry_delay\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeDelta\"\n        },\n        {\n          \"type\": \"null\"\n        }\n\
  \      ]\n    },\n    \"retry_exponential_backoff\": {\n      \"type\": \"number\",\n      \"title\": \"Retry Exponential Backoff\"\n    },\n    \"priority_weight\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Priority Weight\"\n    },\n    \"weight_rule\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Weight Rule\"\n    },\n    \"ui_color\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Ui Color\"\n    },\n    \"ui_fgcolor\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Ui Fgcolor\"\n    },\n    \"template_fields\": {\n      \"anyOf\": [\n\
  \        {\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Template Fields\"\n    },\n    \"downstream_task_ids\": {\n      \"anyOf\": [\n        {\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Downstream Task Ids\"\n    },\n    \"doc_md\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Doc Md\"\n    },\n    \"operator_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Operator Name\"\n    },\n    \"params\": {\n      \"anyOf\": [\n        {\n          \"additionalProperties\"\
  : true,\n          \"type\": \"object\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Params\"\n    },\n    \"class_ref\": {\n      \"anyOf\": [\n        {\n          \"additionalProperties\": true,\n          \"type\": \"object\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Class Ref\"\n    },\n    \"is_mapped\": {\n      \"anyOf\": [\n        {\n          \"type\": \"boolean\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Is Mapped\"\n    },\n    \"extra_links\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Extra Links\",\n      \"description\": \"Extract and return extra_links.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"task_id\",\n    \"task_display_name\",\n    \"owner\",\n    \"start_date\",\n    \"end_date\",\n    \"trigger_rule\",\n    \"depends_on_past\"\
  ,\n    \"wait_for_downstream\",\n    \"retries\",\n    \"queue\",\n    \"pool\",\n    \"pool_slots\",\n    \"execution_timeout\",\n    \"retry_delay\",\n    \"retry_exponential_backoff\",\n    \"priority_weight\",\n    \"weight_rule\",\n    \"ui_color\",\n    \"ui_fgcolor\",\n    \"template_fields\",\n    \"downstream_task_ids\",\n    \"doc_md\",\n    \"operator_name\",\n    \"params\",\n    \"class_ref\",\n    \"is_mapped\",\n    \"extra_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskResponse
---
