---
description: Connection serializer for responses.
layout: schema
name: ConnectionResponse
properties_list:
- description: ''
  name: connection_id
  type: string
- description: ''
  name: conn_type
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: host
  type: object
- description: ''
  name: login
  type: object
- description: ''
  name: schema
  type: object
- description: ''
  name: port
  type: object
- description: ''
  name: password
  type: object
- description: ''
  name: extra
  type: object
- description: ''
  name: team_name
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-connection-response-schema.json
slug: airflow-connection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-connection-response-schema.json\",\n  \"title\": \"ConnectionResponse\",\n  \"description\": \"Connection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connection_id\": {\n      \"type\": \"string\",\n      \"title\": \"Connection Id\"\n    },\n    \"conn_type\": {\n      \"type\": \"string\",\n      \"title\": \"Conn Type\"\n    },\n    \"description\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Description\"\n    },\n    \"host\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Host\"\n    },\n    \"login\": {\n      \"anyOf\": [\n        {\n\
  \          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Login\"\n    },\n    \"schema\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Schema\"\n    },\n    \"port\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Port\"\n    },\n    \"password\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Password\"\n    },\n    \"extra\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Extra\"\n    },\n    \"team_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n\
  \        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Team Name\"\n    }\n  },\n  \"required\": [\n    \"connection_id\",\n    \"conn_type\",\n    \"description\",\n    \"host\",\n    \"login\",\n    \"schema\",\n    \"port\",\n    \"password\",\n    \"extra\",\n    \"team_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-connection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ConnectionResponse
---
