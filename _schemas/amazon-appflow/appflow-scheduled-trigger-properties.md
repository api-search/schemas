---
description: ScheduledTriggerProperties schema from Amazon AppFlow API
layout: schema
name: ScheduledTriggerProperties
properties_list:
- description: The scheduling expression that determines the rate at which the schedule will run, for example rate(5minutes).
  name: scheduleExpression
  type: string
- description: Specifies whether a scheduled flow has an incremental data transfer or a complete data transfer for each flow run.
  name: dataPullMode
  type: string
- description: The time at which the scheduled flow starts.
  name: scheduleStartTime
  type: integer
- description: The time at which the scheduled flow ends.
  name: scheduleEndTime
  type: integer
- description: Specifies the time zone used when referring to the date and time of a scheduled-triggered flow.
  name: timezone
  type: string
- description: Specifies the optional offset that is added to the time interval for a schedule-triggered flow.
  name: scheduleOffset
  type: integer
- description: Specifies the date range for the records to import from the connector in the first flow run.
  name: firstExecutionFrom
  type: integer
- description: Defines how many times a scheduled flow fails consecutively before Amazon AppFlow deactivates it.
  name: flowErrorDeactivationThreshold
  type: integer
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-scheduled-trigger-properties-schema.json
slug: appflow-scheduled-trigger-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-scheduled-trigger-properties-schema.json\",\n  \"title\": \"ScheduledTriggerProperties\",\n  \"description\": \"ScheduledTriggerProperties schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduleExpression\": {\n      \"type\": \"string\",\n      \"example\": \"rate(1day)\",\n      \"description\": \"The scheduling expression that determines the rate at which the schedule will run, for example rate(5minutes).\"\n    },\n    \"dataPullMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Incremental\",\n        \"Complete\"\n      ],\n      \"example\": \"Incremental\",\n      \"description\": \"Specifies whether a scheduled flow has an incremental data transfer or a complete data transfer for each flow run.\"\n    },\n    \"scheduleStartTime\"\
  : {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"The time at which the scheduled flow starts.\"\n    },\n    \"scheduleEndTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"The time at which the scheduled flow ends.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"example\": \"America/New_York\",\n      \"description\": \"Specifies the time zone used when referring to the date and time of a scheduled-triggered flow.\"\n    },\n    \"scheduleOffset\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 0,\n      \"description\": \"Specifies the optional offset that is added to the time interval for a schedule-triggered flow.\"\n    },\n    \"firstExecutionFrom\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993,\n      \"description\": \"\
  Specifies the date range for the records to import from the connector in the first flow run.\"\n    },\n    \"flowErrorDeactivationThreshold\": {\n      \"type\": \"integer\",\n      \"example\": 3,\n      \"description\": \"Defines how many times a scheduled flow fails consecutively before Amazon AppFlow deactivates it.\"\n    }\n  },\n  \"required\": [\n    \"scheduleExpression\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-scheduled-trigger-properties-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ScheduledTriggerProperties
---
