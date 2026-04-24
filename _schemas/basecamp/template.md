---
description: ''
layout: schema
name: Template
properties_list:
- description: Template ID
  name: id
  type: integer
- description: Template status
  name: status
  type: string
- description: Timestamp when the template was created
  name: created_at
  type: string
- description: Timestamp when the template was last updated
  name: updated_at
  type: string
- description: Template name
  name: name
  type: string
- description: Template description
  name: description
  type: string
- description: API URL for this template
  name: url
  type: string
- description: Web URL for this template
  name: app_url
  type: string
- description: Tools available in this template
  name: dock
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/template-schema.json
slug: template
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Template
---
