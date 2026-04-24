---
description: An organizational department from a connected HRIS system.
layout: schema
name: Department
properties_list:
- description: Department ID.
  name: id
  type: string
- description: Department name.
  name: name
  type: string
- description: Parent department ID for nested structures.
  name: parent_id
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-department-schema.json
slug: bindbee-department
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: Department
---
