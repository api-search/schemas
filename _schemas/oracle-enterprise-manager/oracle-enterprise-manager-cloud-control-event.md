---
description: Represents a monitoring event detected by Enterprise Manager. Events are the atomic detections that are correlated into incidents.
layout: schema
name: Event
properties_list:
- description: Unique identifier of the event.
  name: eventId
  type: string
- description: Type of the event.
  name: eventType
  type: string
- description: Severity of the event.
  name: severity
  type: string
- description: Descriptive message for the event.
  name: message
  type: string
- description: Name of the target that generated this event.
  name: targetName
  type: string
- description: Type of the target that generated this event.
  name: targetType
  type: string
- description: Name of the metric group, if this is a metric alert event.
  name: metricGroupName
  type: string
- description: Name of the metric column, if this is a metric alert event.
  name: metricColumnName
  type: string
- description: Metric value that triggered the event.
  name: metricValue
  type: number
- description: Timestamp when the event was raised.
  name: timeRaised
  type: string
- description: Timestamp when the event was resolved.
  name: timeResolved
  type: string
- description: Canonical URI for this event resource.
  name: canonicalLink
  type: string
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-event-schema.json
slug: oracle-enterprise-manager-cloud-control-event
source_filename: oracle-enterprise-manager-cloud-control-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Event\",\n  \"type\": \"object\",\n  \"description\": \"Represents a monitoring event detected by Enterprise Manager. Events are the atomic detections that are correlated into incidents.\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the event.\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the event.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity of the event.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Descriptive message for the event.\"\n    },\n    \"targetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target that generated this event.\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the target that generated\
  \ this event.\"\n    },\n    \"metricGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the metric group, if this is a metric alert event.\"\n    },\n    \"metricColumnName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the metric column, if this is a metric alert event.\"\n    },\n    \"metricValue\": {\n      \"type\": \"number\",\n      \"description\": \"Metric value that triggered the event.\"\n    },\n    \"timeRaised\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the event was raised.\"\n    },\n    \"timeResolved\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the event was resolved.\"\n    },\n    \"canonicalLink\": {\n      \"type\": \"string\",\n      \"description\": \"Canonical URI for this event resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-event-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: Event
---
