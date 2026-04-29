---
description: Asset event serializer for responses.
layout: schema
name: AssetEventResponse
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: asset_id
  type: integer
- description: ''
  name: uri
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: group
  type: object
- description: ''
  name: extra
  type: object
- description: ''
  name: source_task_id
  type: object
- description: ''
  name: source_dag_id
  type: object
- description: ''
  name: source_run_id
  type: object
- description: ''
  name: source_map_index
  type: integer
- description: ''
  name: created_dagruns
  type: array
- description: ''
  name: timestamp
  type: string
- description: ''
  name: partition_key
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-asset-event-response-schema.json
slug: airflow-asset-event-response
source_filename: airflow-asset-event-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-event-response-schema.json\",\n  \"title\": \"AssetEventResponse\",\n  \"description\": \"Asset event serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"title\": \"Id\"\n    },\n    \"asset_id\": {\n      \"type\": \"integer\",\n      \"title\": \"Asset Id\"\n    },\n    \"uri\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Uri\"\n    },\n    \"name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Name\"\n    },\n    \"group\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n   \
  \     },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Group\"\n    },\n    \"extra\": {\n      \"anyOf\": [\n        {\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/JsonValue\"\n          },\n          \"type\": \"object\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Extra\"\n    },\n    \"source_task_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Source Task Id\"\n    },\n    \"source_dag_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Source Dag Id\"\n    },\n    \"source_run_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\"\
  : \"Source Run Id\"\n    },\n    \"source_map_index\": {\n      \"type\": \"integer\",\n      \"title\": \"Source Map Index\"\n    },\n    \"created_dagruns\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DagRunAssetReference\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Created Dagruns\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Timestamp\"\n    },\n    \"partition_key\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Partition Key\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"asset_id\",\n    \"source_map_index\",\n    \"created_dagruns\",\n    \"timestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-event-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: AssetEventResponse
---
