---
description: Schema representing the AppDynamics application monitoring model including applications, tiers, nodes, business transactions, and backends.
layout: schema
name: AppDynamics Application Model
properties_list:
- description: The list of monitored business applications.
  name: applications
  type: array
- description: The list of tiers within the application.
  name: tiers
  type: array
- description: The list of nodes within the application.
  name: nodes
  type: array
- description: The list of business transactions detected in the application.
  name: businessTransactions
  type: array
- description: The list of backend components detected in the application.
  name: backends
  type: array
provider_name: AppDynamics
provider_slug: appdynamics
schema_file: json-schema/appdynamics-application-model-schema.json
slug: appdynamics-application-model
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
title: AppDynamics Application Model
---
