---
description: A job candidate from a connected ATS system.
layout: schema
name: Candidate
properties_list:
- description: Candidate ID.
  name: id
  type: string
- description: Candidate first name.
  name: first_name
  type: string
- description: Candidate last name.
  name: last_name
  type: string
- description: Candidate email.
  name: email
  type: string
- description: Job ID the candidate applied for.
  name: job_id
  type: string
- description: Current hiring stage.
  name: stage
  type: string
- description: Application creation timestamp.
  name: created_at
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-candidate-schema.json
slug: bindbee-candidate
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: Candidate
---
