---
description: TriggerConfig schema from Amazon AppFlow API
layout: schema
name: TriggerConfig
properties_list:
- description: Specifies the type of flow trigger. It can be OnDemand, Scheduled, or Event.
  name: triggerType
  type: string
- description: Specifies the configuration details of a schedule-triggered flow as defined by the user.
  name: triggerProperties
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-trigger-config-schema.json
slug: appflow-trigger-config
source_filename: appflow-trigger-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-trigger-config-schema.json\",\n  \"title\": \"TriggerConfig\",\n  \"description\": \"TriggerConfig schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"triggerType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Scheduled\",\n        \"Event\",\n        \"OnDemand\"\n      ],\n      \"example\": \"Scheduled\",\n      \"description\": \"Specifies the type of flow trigger. It can be OnDemand, Scheduled, or Event.\"\n    },\n    \"triggerProperties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Scheduled\": {}\n      },\n      \"description\": \"Specifies the configuration details of a schedule-triggered flow as defined by the user.\"\n    }\n  },\n  \"required\": [\n    \"triggerType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-trigger-config-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: TriggerConfig
---
