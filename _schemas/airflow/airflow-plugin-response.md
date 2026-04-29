---
description: Plugin serializer.
layout: schema
name: PluginResponse
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: macros
  type: array
- description: ''
  name: flask_blueprints
  type: array
- description: ''
  name: fastapi_apps
  type: array
- description: ''
  name: fastapi_root_middlewares
  type: array
- description: Aggregate all external views. Both 'external_views' and 'appbuilder_menu_items' are included here.
  name: external_views
  type: array
- description: ''
  name: react_apps
  type: array
- description: ''
  name: appbuilder_views
  type: array
- description: ''
  name: appbuilder_menu_items
  type: array
- description: ''
  name: global_operator_extra_links
  type: array
- description: ''
  name: operator_extra_links
  type: array
- description: ''
  name: source
  type: string
- description: ''
  name: listeners
  type: array
- description: ''
  name: timetables
  type: array
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-plugin-response-schema.json
slug: airflow-plugin-response
source_filename: airflow-plugin-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-plugin-response-schema.json\",\n  \"title\": \"PluginResponse\",\n  \"description\": \"Plugin serializer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"macros\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Macros\"\n    },\n    \"flask_blueprints\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Flask Blueprints\"\n    },\n    \"fastapi_apps\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FastAPIAppResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Fastapi Apps\"\n    },\n    \"fastapi_root_middlewares\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FastAPIRootMiddlewareResponse\"\
  \n      },\n      \"type\": \"array\",\n      \"title\": \"Fastapi Root Middlewares\"\n    },\n    \"external_views\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ExternalViewResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"External Views\",\n      \"description\": \"Aggregate all external views. Both 'external_views' and 'appbuilder_menu_items' are included here.\"\n    },\n    \"react_apps\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ReactAppResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"React Apps\"\n    },\n    \"appbuilder_views\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AppBuilderViewResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Appbuilder Views\"\n    },\n    \"appbuilder_menu_items\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AppBuilderMenuItemResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Appbuilder Menu\
  \ Items\",\n      \"deprecated\": true\n    },\n    \"global_operator_extra_links\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Global Operator Extra Links\"\n    },\n    \"operator_extra_links\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Operator Extra Links\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"title\": \"Source\"\n    },\n    \"listeners\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Listeners\"\n    },\n    \"timetables\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Timetables\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"macros\",\n    \"flask_blueprints\",\n    \"fastapi_apps\",\n    \"fastapi_root_middlewares\",\n    \"external_views\",\n    \"react_apps\",\n    \"appbuilder_views\"\
  ,\n    \"appbuilder_menu_items\",\n    \"global_operator_extra_links\",\n    \"operator_extra_links\",\n    \"source\",\n    \"listeners\",\n    \"timetables\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-plugin-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: PluginResponse
---
