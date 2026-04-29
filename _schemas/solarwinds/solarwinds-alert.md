---
description: Schema for a SolarWinds monitoring alert triggered by threshold violations or status changes on monitored entities.
layout: schema
name: SolarWinds Alert
properties_list:
- description: Unique identifier for the alert instance
  name: alertId
  type: integer
- description: Display name of the alert definition
  name: alertName
  type: string
- description: Alert severity level
  name: severity
  type: string
- description: Timestamp when the alert was triggered
  name: triggeredAt
  type: string
- description: Timestamp when the alert was reset, null if still active
  name: resetAt
  type:
  - string
  - 'null'
- description: Whether the alert has been acknowledged by an operator
  name: acknowledged
  type: boolean
- description: Username of the operator who acknowledged the alert
  name: acknowledgedBy
  type:
  - string
  - 'null'
- description: Alert message with details about the triggering condition
  name: message
  type: string
- description: Type of the monitored entity that triggered the alert
  name: entityType
  type: string
- description: SWIS URI of the entity that triggered the alert
  name: entityUri
  type: string
- description: Display name of the triggering entity
  name: entityCaption
  type: string
- description: ''
  name: triggerCondition
  type: object
- description: Additional notes or annotations on the alert
  name: notes
  type: string
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-alert-schema.json
slug: solarwinds-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://solarwinds.com/schemas/solarwinds/alert.json\",\n  \"title\": \"SolarWinds Alert\",\n  \"description\": \"Schema for a SolarWinds monitoring alert triggered by threshold violations or status changes on monitored entities.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"alertId\",\n    \"alertName\",\n    \"severity\",\n    \"triggeredAt\"\n  ],\n  \"properties\": {\n    \"alertId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the alert instance\"\n    },\n    \"alertName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the alert definition\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Alert severity level\",\n      \"enum\": [\n        \"Information\",\n        \"Warning\",\n        \"Critical\",\n        \"Serious\",\n        \"Notice\"\n      ]\n    },\n    \"triggeredAt\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alert was triggered\"\n    },\n    \"resetAt\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the alert was reset, null if still active\"\n    },\n    \"acknowledged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the alert has been acknowledged by an operator\",\n      \"default\": false\n    },\n    \"acknowledgedBy\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Username of the operator who acknowledged the alert\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Alert message with details about the triggering condition\"\n    },\n    \"entityType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the monitored entity that triggered the alert\",\n      \"examples\": [\n        \"Orion.Nodes\",\n        \"Orion.Volumes\"\
  ,\n        \"Orion.NPM.Interfaces\"\n      ]\n    },\n    \"entityUri\": {\n      \"type\": \"string\",\n      \"description\": \"SWIS URI of the entity that triggered the alert\"\n    },\n    \"entityCaption\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the triggering entity\"\n    },\n    \"triggerCondition\": {\n      \"$ref\": \"#/$defs/TriggerCondition\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Additional notes or annotations on the alert\"\n    }\n  },\n  \"$defs\": {\n    \"TriggerCondition\": {\n      \"type\": \"object\",\n      \"description\": \"Condition that caused the alert to trigger\",\n      \"properties\": {\n        \"property\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the monitored property\"\n        },\n        \"operator\": {\n          \"type\": \"string\",\n          \"description\": \"Comparison operator\",\n          \"enum\": [\n            \"Greater Than\"\
  ,\n            \"Less Than\",\n            \"Equal To\",\n            \"Not Equal To\",\n            \"Greater Than or Equal To\",\n            \"Less Than or Equal To\"\n          ]\n        },\n        \"threshold\": {\n          \"type\": \"number\",\n          \"description\": \"Threshold value that was exceeded\"\n        },\n        \"currentValue\": {\n          \"type\": \"number\",\n          \"description\": \"Current value of the monitored property\"\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"description\": \"Duration in seconds the condition must persist before triggering\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-alert-schema.json
tags:
- Application Monitoring
- Database Monitoring
- Infrastructure
- IP Address Management
- IT Management
- ITSM
- Log Management
- Network Monitoring
- Observability
title: SolarWinds Alert
---
