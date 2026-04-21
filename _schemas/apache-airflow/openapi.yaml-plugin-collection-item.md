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
