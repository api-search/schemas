---
description: Represents a telemetry record for sending unit metric or allocation data to CloudZero for cost analysis and unit economics calculations.
layout: schema
name: CloudZero Telemetry Record
properties_list:
- description: Timestamp for the telemetry record.
  name: timestamp
  type: string
- description: Numeric value for the metric or allocation.
  name: value
  type: number
- description: Time granularity of the record.
  name: granularity
  type: string
- description: Key-value pairs for filtering and grouping unit metric telemetry.
  name: filter
  type: object
- description: Key-value pairs identifying the element being allocated for allocation telemetry.
  name: element
  type: object
provider_name: CloudZero
provider_slug: cloudzero
schema_file: json-schema/cloudzero-telemetry-record.json
slug: cloudzero-telemetry-record
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
title: CloudZero Telemetry Record
---
