---
description: ''
layout: schema
name: ProjectConstruction
properties_list:
- description: Project construction job ID
  name: id
  type: integer
- description: Construction status
  name: status
  type: string
- description: API URL to poll for this construction job
  name: url
  type: string
- description: The resulting project once construction is completed
  name: project
  type: object
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/projectconstruction-schema.json
slug: projectconstruction
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: ProjectConstruction
---
