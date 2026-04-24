---
description: Paginated list of employee records.
layout: schema
name: EmployeesResponse
properties_list:
- description: Array of employee records.
  name: data
  type: array
- description: Cursor for next page.
  name: next_cursor
  type: string
- description: Whether more records exist.
  name: has_more
  type: boolean
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-employees-response-schema.json
slug: bindbee-employees-response
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: EmployeesResponse
---
