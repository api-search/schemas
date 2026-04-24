---
description: A normalized employee record from a connected HRIS system.
layout: schema
name: Employee
properties_list:
- description: Bindbee employee ID.
  name: id
  type: string
- description: Employee first name.
  name: first_name
  type: string
- description: Employee last name.
  name: last_name
  type: string
- description: Employee work email.
  name: email
  type: string
- description: Job title.
  name: job_title
  type: string
- description: Department name.
  name: department
  type: string
- description: Employment status.
  name: employment_status
  type: string
- description: Employment start date.
  name: start_date
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-employee-schema.json
slug: bindbee-employee
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: Employee
---
