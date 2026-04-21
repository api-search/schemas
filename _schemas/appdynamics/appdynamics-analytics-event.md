---
description: Schema representing a custom analytics event and its schema definition for the AppDynamics Events Service.
layout: schema
name: AppDynamics Analytics Event
properties_list:
- description: The name of the custom event schema.
  name: schemaName
  type: string
- description: The schema definition for this event type.
  name: schema
  type: object
- description: Array of event data objects conforming to the schema.
  name: events
  type: array
provider_name: AppDynamics
provider_slug: appdynamics
schema_file: json-schema/appdynamics-analytics-event-schema.json
slug: appdynamics-analytics-event
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
title: AppDynamics Analytics Event
---
