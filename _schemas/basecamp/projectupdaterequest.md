---
description: ''
layout: schema
name: ProjectUpdateRequest
properties_list:
- description: Updated project name
  name: name
  type: string
- description: Updated project description
  name: description
  type: string
- description: Optional schedule date range for the project
  name: schedule_attributes
  type: object
- description: Controls who can join the project
  name: admissions
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/projectupdaterequest-schema.json
slug: projectupdaterequest
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProjectUpdateRequest
---
