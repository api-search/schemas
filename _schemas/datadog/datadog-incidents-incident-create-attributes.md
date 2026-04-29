---
description: Attributes for creating a new incident
layout: schema
name: IncidentCreateAttributes
properties_list:
- description: The title of the incident describing what is affected and the nature of the issue
  name: title
  type: string
- description: Whether the incident is causing direct customer impact (required field for all incidents)
  name: customer_impacted
  type: boolean
- description: Description of the customer groups or features affected by this incident
  name: customer_impact_scope
  type: string
- description: ISO 8601 timestamp when customer impact started, if known
  name: customer_impact_start
  type: string
- description: The severity level of the incident using SEV-N notation
  name: severity
  type: string
- description: The initial state of the incident
  name: state
  type: string
- description: Custom fields for the incident as configured in your organization settings
  name: fields
  type: object
- description: List of user and team notification handles to page on incident creation
  name: notification_handles
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-create-attributes-schema.json
slug: datadog-incidents-incident-create-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-create-attributes-schema.json\",\n  \"title\": \"IncidentCreateAttributes\",\n  \"description\": \"Attributes for creating a new incident\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the incident describing what is affected and the nature of the issue\",\n      \"example\": \"Example Monitor\"\n    },\n    \"customer_impacted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the incident is causing direct customer impact (required field for all incidents)\",\n      \"example\": true\n    },\n    \"customer_impact_scope\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the customer groups or features affected by this incident\",\n      \"example\": \"example_value\"\
  \n    },\n    \"customer_impact_start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when customer impact started, if known\",\n      \"example\": \"example_value\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity level of the incident using SEV-N notation\",\n      \"enum\": [\n        \"SEV-1\",\n        \"SEV-2\",\n        \"SEV-3\",\n        \"SEV-4\",\n        \"SEV-5\",\n        \"UNKNOWN\"\n      ],\n      \"example\": \"SEV-1\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The initial state of the incident\",\n      \"enum\": [\n        \"active\",\n        \"stable\",\n        \"resolved\"\n      ],\n      \"default\": \"active\",\n      \"example\": \"active\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom fields for the incident as configured in your organization settings\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"object\"\n      }\n    },\n    \"notification_handles\": {\n      \"type\": \"array\",\n      \"description\": \"List of user and team notification handles to page on incident creation\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"handle\": {\n            \"type\": \"string\",\n            \"description\": \"The Datadog handle or integration channel to notify\"\n          },\n          \"display_name\": {\n            \"type\": \"string\",\n            \"description\": \"The display name for this notification handle\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"customer_impacted\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-create-attributes-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentCreateAttributes
---
