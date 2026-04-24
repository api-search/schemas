---
description: An employee time-off request from a connected HRIS system.
layout: schema
name: TimeOffRequest
properties_list:
- description: Time-off request ID.
  name: id
  type: string
- description: Employee ID.
  name: employee_id
  type: string
- description: Type of time off.
  name: type
  type: string
- description: Approval status.
  name: status
  type: string
- description: Time-off start date.
  name: start_date
  type: string
- description: Time-off end date.
  name: end_date
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-time-off-request-schema.json
slug: bindbee-time-off-request
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: TimeOffRequest
---
