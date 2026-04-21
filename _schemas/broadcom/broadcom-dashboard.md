---
description: A Dashboard represents a configurable visualization in Operations for Applications that displays metric data through charts, tables, and other widgets for monitoring and analysis.
layout: schema
name: Broadcom Dashboard
properties_list:
- description: The unique identifier of the dashboard.
  name: id
  type: string
- description: The display name of the dashboard.
  name: name
  type: string
- description: A description of the dashboard.
  name: description
  type: string
- description: The URL slug used to access the dashboard.
  name: url
  type: string
- description: Tags associated with the dashboard.
  name: tags
  type: object
- description: The sections of the dashboard containing rows of charts.
  name: sections
  type: array
- description: The identifier of the user who created the dashboard.
  name: creatorId
  type: string
- description: The identifier of the user who last updated the dashboard.
  name: updaterId
  type: string
- description: The creation timestamp in epoch milliseconds.
  name: createdEpochMillis
  type: integer
- description: The last update timestamp in epoch milliseconds.
  name: updatedEpochMillis
  type: integer
- description: Dashboard parameters for dynamic filtering.
  name: parameters
  type: object
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-dashboard-schema.json
slug: broadcom-dashboard
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Dashboard
---
