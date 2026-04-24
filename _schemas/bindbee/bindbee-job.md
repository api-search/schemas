---
description: A job posting from a connected ATS system.
layout: schema
name: Job
properties_list:
- description: Job ID.
  name: id
  type: string
- description: Job title.
  name: title
  type: string
- description: Hiring department.
  name: department
  type: string
- description: Job location or remote.
  name: location
  type: string
- description: Job posting status.
  name: status
  type: string
- description: Job creation timestamp.
  name: created_at
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-job-schema.json
slug: bindbee-job
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: Job
---
