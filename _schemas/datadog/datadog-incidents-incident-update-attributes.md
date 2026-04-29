---
description: Attributes to update on an existing incident
layout: schema
name: IncidentUpdateAttributes
properties_list:
- description: The updated title of the incident
  name: title
  type: string
- description: The updated state of the incident (transitioning to resolved records resolution time)
  name: state
  type: string
- description: The updated severity level of the incident
  name: severity
  type: string
- description: Updated flag indicating whether the incident has customer impact
  name: customer_impacted
  type: boolean
- description: Updated description of the customer impact scope
  name: customer_impact_scope
  type: string
- description: ISO 8601 timestamp when customer impact ended (set when marking impact as resolved)
  name: customer_impact_end
  type: string
- description: Updated custom field values for the incident
  name: fields
  type: object
- description: Updated list of notification handles for the incident
  name: notification_handles
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incident-update-attributes-schema.json
slug: datadog-incidents-incident-update-attributes
source_filename: datadog-incidents-incident-update-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-update-attributes-schema.json\",\n  \"title\": \"IncidentUpdateAttributes\",\n  \"description\": \"Attributes to update on an existing incident\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The updated title of the incident\",\n      \"example\": \"Example Monitor\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The updated state of the incident (transitioning to resolved records resolution time)\",\n      \"enum\": [\n        \"active\",\n        \"stable\",\n        \"resolved\"\n      ],\n      \"example\": \"active\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The updated severity level of the incident\",\n      \"enum\": [\n      \
  \  \"SEV-1\",\n        \"SEV-2\",\n        \"SEV-3\",\n        \"SEV-4\",\n        \"SEV-5\",\n        \"UNKNOWN\"\n      ],\n      \"example\": \"SEV-1\"\n    },\n    \"customer_impacted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Updated flag indicating whether the incident has customer impact\",\n      \"example\": true\n    },\n    \"customer_impact_scope\": {\n      \"type\": \"string\",\n      \"description\": \"Updated description of the customer impact scope\",\n      \"example\": \"example_value\"\n    },\n    \"customer_impact_end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when customer impact ended (set when marking impact as resolved)\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Updated custom field values for the incident\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n   \
  \ \"notification_handles\": {\n      \"type\": \"array\",\n      \"description\": \"Updated list of notification handles for the incident\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incident-update-attributes-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentUpdateAttributes
---
