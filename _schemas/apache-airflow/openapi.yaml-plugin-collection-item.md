---
description: A plugin Item. *New in version 2.1.0*
layout: schema
name: PluginCollectionItem
properties_list:
- description: The Flask Appbuilder menu items
  name: appbuilder_menu_items
  type: array
- description: The appuilder views
  name: appbuilder_views
  type: array
- description: The plugin executors
  name: executors
  type: array
- description: The flask blueprints
  name: flask_blueprints
  type: array
- description: The global operator extra links
  name: global_operator_extra_links
  type: array
- description: The plugin hooks
  name: hooks
  type: array
- description: The plugin macros
  name: macros
  type: array
- description: The name of the plugin
  name: name
  type: string
- description: Operator extra links
  name: operator_extra_links
  type: array
- description: The plugin source
  name: source
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-plugin-collection-item-schema.json
slug: openapi.yaml-plugin-collection-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-plugin-collection-item-schema.json\",\n  \"title\": \"PluginCollectionItem\",\n  \"description\": \"A plugin Item.\\n\\n*New in version 2.1.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appbuilder_menu_items\": {\n      \"description\": \"The Flask Appbuilder menu items\",\n      \"items\": {\n        \"nullable\": true,\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"appbuilder_views\": {\n      \"description\": \"The appuilder views\",\n      \"items\": {\n        \"nullable\": true,\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"executors\": {\n      \"description\": \"The plugin executors\",\n      \"items\": {\n        \"nullable\": true,\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\
  \n    },\n    \"flask_blueprints\": {\n      \"description\": \"The flask blueprints\",\n      \"items\": {\n        \"nullable\": true,\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"global_operator_extra_links\": {\n      \"description\": \"The global operator extra links\",\n      \"items\": {\n        \"nullable\": true,\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"hooks\": {\n      \"description\": \"The plugin hooks\",\n      \"items\": {\n        \"nullable\": true,\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"macros\": {\n      \"description\": \"The plugin macros\",\n      \"items\": {\n        \"nullable\": true,\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"name\": {\n      \"description\": \"The name of the plugin\",\n      \"type\": \"string\"\n    },\n    \"operator_extra_links\": {\n      \"description\": \"Operator extra links\"\
  ,\n      \"items\": {\n        \"nullable\": true,\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"source\": {\n      \"description\": \"The plugin source\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-plugin-collection-item-schema.json
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
title: PluginCollectionItem
---
