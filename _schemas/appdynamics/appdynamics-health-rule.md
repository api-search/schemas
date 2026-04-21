---
description: Schema representing an AppDynamics health rule configuration that defines performance thresholds, violation conditions, and evaluation criteria for monitored entities.
layout: schema
name: AppDynamics Health Rule
properties_list:
- description: The internal numeric identifier for the health rule.
  name: id
  type: integer
- description: The name of the health rule.
  name: name
  type: string
- description: Whether the health rule is currently enabled.
  name: enabled
  type: boolean
- description: The evaluation time window in minutes.
  name: useDataFromLastNMinutes
  type: integer
- description: Time in minutes to wait after a violation before re-evaluating.
  name: waitTimeAfterViolation
  type: integer
- description: The schedule name that determines when this health rule is active.
  name: scheduleName
  type: string
- description: Defines which entities are affected by this health rule.
  name: affects
  type: object
- description: The evaluation criteria containing critical and warning conditions.
  name: evalCriterias
  type: object
provider_name: AppDynamics
provider_slug: appdynamics
schema_file: json-schema/appdynamics-health-rule-schema.json
slug: appdynamics-health-rule
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
title: AppDynamics Health Rule
---
