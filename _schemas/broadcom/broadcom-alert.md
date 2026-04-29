---
description: An Alert represents a configurable monitoring rule in Operations for Applications that evaluates metric conditions and triggers notifications when thresholds are breached.
layout: schema
name: Broadcom Alert
properties_list:
- description: The unique identifier of the alert.
  name: id
  type: string
- description: The display name of the alert.
  name: name
  type: string
- description: The query expression that defines the alert condition.
  name: condition
  type: string
- description: The query expression used for display purposes in notifications.
  name: displayExpression
  type: string
- description: The number of minutes the condition must be met before the alert fires.
  name: minutes
  type: integer
- description: The number of minutes after which the alert auto-resolves if the condition clears.
  name: resolveAfterMinutes
  type: integer
- description: The severity level of the alert.
  name: severity
  type: string
- description: The current statuses of the alert.
  name: status
  type: array
- description: Tags associated with the alert.
  name: tags
  type: object
- description: Notification targets keyed by severity level.
  name: targets
  type: object
- description: The identifier of the user who created the alert.
  name: creatorId
  type: string
- description: The identifier of the user who last updated the alert.
  name: updaterId
  type: string
- description: The creation timestamp in epoch milliseconds.
  name: createdEpochMillis
  type: integer
- description: The last update timestamp in epoch milliseconds.
  name: updatedEpochMillis
  type: integer
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-alert-schema.json
slug: broadcom-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/broadcom/blob/main/json-schema/broadcom-alert-schema.json\",\n  \"title\": \"Broadcom Alert\",\n  \"description\": \"An Alert represents a configurable monitoring rule in Operations for Applications that evaluates metric conditions and triggers notifications when thresholds are breached.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the alert.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the alert.\"\n    },\n    \"condition\": {\n      \"type\": \"string\",\n      \"description\": \"The query expression that defines the alert condition.\"\n    },\n    \"displayExpression\": {\n      \"type\": \"string\",\n      \"description\": \"The query expression used for display purposes in notifications.\"\n    },\n \
  \   \"minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of minutes the condition must be met before the alert fires.\"\n    },\n    \"resolveAfterMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of minutes after which the alert auto-resolves if the condition clears.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INFO\",\n        \"SMOKE\",\n        \"WARN\",\n        \"SEVERE\"\n      ],\n      \"description\": \"The severity level of the alert.\"\n    },\n    \"status\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"CHECKING\",\n          \"FIRING\",\n          \"NO_DATA\",\n          \"SNOOZED\",\n          \"TRASH\",\n          \"IN_MAINTENANCE\"\n        ]\n      },\n      \"description\": \"The current statuses of the alert.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"properties\": {\n    \
  \    \"customerTags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"User-defined tags for the alert.\"\n        }\n      },\n      \"description\": \"Tags associated with the alert.\"\n    },\n    \"targets\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"Notification targets keyed by severity level.\"\n    },\n    \"creatorId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user who created the alert.\"\n    },\n    \"updaterId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user who last updated the alert.\"\n    },\n    \"createdEpochMillis\": {\n      \"type\": \"integer\",\n      \"description\": \"The creation timestamp in epoch milliseconds.\"\n    },\n    \"updatedEpochMillis\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The last update timestamp in epoch milliseconds.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/json-schema/broadcom-alert-schema.json
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Alert
---
