---
description: An alert event representing a triggered alert condition on an SAP HANA Cloud service instance. Alerts monitor database health, resources, and operational thresholds.
layout: schema
name: AlertEvent
properties_list:
- description: The unique identifier of the alert event.
  name: alertId
  type: string
- description: The identifier of the alert rule that triggered this event.
  name: alertRuleId
  type: string
- description: The human-readable name of the alert (e.g., Memory Usage, Disk Usage, Long-Running Statements).
  name: alertName
  type: string
- description: The current state of the alert event.
  name: alertState
  type: string
- description: The severity level of the alert.
  name: severity
  type: string
- description: A detailed description of the alert condition.
  name: description
  type: string
- description: ISO 8601 timestamp when the alert was triggered.
  name: triggeredAt
  type: string
- description: ISO 8601 timestamp when the alert was resolved. Null if the alert is still active.
  name: resolvedAt
  type: string
- description: The current metric value that triggered or relates to the alert.
  name: currentValue
  type: number
- description: The threshold value configured in the alert rule.
  name: thresholdValue
  type: number
- description: The unit of measurement for the metric values (e.g., %, GB, count).
  name: unit
  type: string
- description: The service instance identifier associated with this alert.
  name: serviceInstanceId
  type: string
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-alert-event-schema.json
slug: sap-hana-cloud-rest-alert-event
source_filename: sap-hana-cloud-rest-alert-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlertEvent\",\n  \"type\": \"object\",\n  \"description\": \"An alert event representing a triggered alert condition on an SAP HANA Cloud service instance. Alerts monitor database health, resources, and operational thresholds.\",\n  \"properties\": {\n    \"alertId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the alert event.\"\n    },\n    \"alertRuleId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the alert rule that triggered this event.\"\n    },\n    \"alertName\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the alert (e.g., Memory Usage, Disk Usage, Long-Running Statements).\"\n    },\n    \"alertState\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the alert event.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The severity level of the alert.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the alert condition.\"\n    },\n    \"triggeredAt\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the alert was triggered.\"\n    },\n    \"resolvedAt\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the alert was resolved. Null if the alert is still active.\"\n    },\n    \"currentValue\": {\n      \"type\": \"number\",\n      \"description\": \"The current metric value that triggered or relates to the alert.\"\n    },\n    \"thresholdValue\": {\n      \"type\": \"number\",\n      \"description\": \"The threshold value configured in the alert rule.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of measurement for the metric values (e.g., %, GB, count).\"\n    },\n    \"serviceInstanceId\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The service instance identifier associated with this alert.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-alert-event-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: AlertEvent
---
