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
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Alert
---
