---
description: The attributes of an incident record
layout: schema
name: IncidentAttributes
properties_list:
- description: The title of the incident describing what is affected
  name: title
  type: string
- description: The sequential human-readable public ID of the incident within the organization
  name: public_id
  type: integer
- description: The current state of the incident in its lifecycle
  name: state
  type: string
- description: The severity level of the incident
  name: severity
  type: string
- description: Whether the incident is causing direct customer impact
  name: customer_impacted
  type: boolean
- description: Description of the scope of customer impact for this incident
  name: customer_impact_scope
  type: string
- description: ISO 8601 timestamp when customer impact began
  name: customer_impact_start
  type: string
- description: ISO 8601 timestamp when customer impact ended
  name: customer_impact_end
  type: string
- description: Duration of customer impact in seconds
  name: customer_impact_duration
  type: integer
- description: ISO 8601 timestamp when the incident was created
  name: created
  type: string
- description: ISO 8601 timestamp when the incident was last modified
  name: modified
  type: string
- description: ISO 8601 timestamp when the incident was first detected
  name: detected
  type: string
- description: ISO 8601 timestamp when the incident was marked as resolved
  name: resolved
  type: string
- description: Time in seconds from incident start to detection
  name: time_to_detect
  type: integer
- description: Time in seconds from detection to first responder acknowledgement
  name: time_to_internal_response
  type: integer
- description: Time in seconds from detection to resolution
  name: time_to_repair
  type: integer
- description: Custom field values for the incident as defined in organization settings
  name: fields
  type: object
- description: List of notification handles that were paged for this incident
  name: notification_handles
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-attributes-schema.json
slug: datadog-incidents-incident-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-attributes-schema.json\",\n  \"title\": \"IncidentAttributes\",\n  \"description\": \"The attributes of an incident record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the incident describing what is affected\",\n      \"example\": \"Example Monitor\"\n    },\n    \"public_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The sequential human-readable public ID of the incident within the organization\",\n      \"example\": 42\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the incident in its lifecycle\",\n      \"enum\": [\n        \"active\",\n        \"stable\",\n        \"resolved\"\n      ],\n      \"example\": \"active\"\n\
  \    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity level of the incident\",\n      \"enum\": [\n        \"SEV-1\",\n        \"SEV-2\",\n        \"SEV-3\",\n        \"SEV-4\",\n        \"SEV-5\",\n        \"UNKNOWN\"\n      ],\n      \"example\": \"SEV-1\"\n    },\n    \"customer_impacted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the incident is causing direct customer impact\",\n      \"example\": true\n    },\n    \"customer_impact_scope\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the scope of customer impact for this incident\",\n      \"example\": \"example_value\"\n    },\n    \"customer_impact_start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when customer impact began\",\n      \"example\": \"example_value\"\n    },\n    \"customer_impact_end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n\
  \      \"description\": \"ISO 8601 timestamp when customer impact ended\",\n      \"example\": \"example_value\"\n    },\n    \"customer_impact_duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration of customer impact in seconds\",\n      \"example\": 42\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the incident was created\",\n      \"example\": \"example_value\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the incident was last modified\",\n      \"example\": \"example_value\"\n    },\n    \"detected\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the incident was first detected\",\n      \"example\": \"example_value\"\n    },\n    \"resolved\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"ISO 8601 timestamp when the incident was marked as resolved\",\n      \"example\": \"example_value\"\n    },\n    \"time_to_detect\": {\n      \"type\": \"integer\",\n      \"description\": \"Time in seconds from incident start to detection\",\n      \"example\": 42\n    },\n    \"time_to_internal_response\": {\n      \"type\": \"integer\",\n      \"description\": \"Time in seconds from detection to first responder acknowledgement\",\n      \"example\": 42\n    },\n    \"time_to_repair\": {\n      \"type\": \"integer\",\n      \"description\": \"Time in seconds from detection to resolution\",\n      \"example\": 42\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom field values for the incident as defined in organization settings\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n    \"notification_handles\": {\n      \"type\": \"array\",\n      \"description\": \"List of notification handles\
  \ that were paged for this incident\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-attributes-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentAttributes
---
