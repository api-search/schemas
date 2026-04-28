---
description: Represents a cost data record returned by the CloudZero Billing API, including grouped dimensions and time-series cost values.
layout: schema
name: CloudZero Cost
properties_list:
- description: Key-value pairs representing the dimensions this cost record is grouped by (e.g., Account, Service, Region).
  name: group
  type: object
- description: Time-series array of cost data points.
  name: cost
  type: array
provider_name: CloudZero
provider_slug: cloudzero
schema_file: json-schema/cloudzero-cost.json
slug: cloudzero-cost
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
title: CloudZero Cost
---
