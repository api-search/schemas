---
description: ''
layout: schema
name: Project
properties_list:
- description: Unique project identifier
  name: id
  type: integer
- description: Project status (active, archived, trashed)
  name: status
  type: string
- description: Timestamp when the project was created
  name: created_at
  type: string
- description: Timestamp when the project was last updated
  name: updated_at
  type: string
- description: Project name
  name: name
  type: string
- description: Project description
  name: description
  type: string
- description: Project purpose classification
  name: purpose
  type: string
- description: Whether client access is enabled for this project
  name: clients_enabled
  type: boolean
- description: Whether timesheets are enabled for this project
  name: timesheet_enabled
  type: boolean
- description: Project color identifier
  name: color
  type: string
- description: API URL for this project
  name: url
  type: string
- description: Web URL for this project
  name: app_url
  type: string
- description: API URL to bookmark this project
  name: bookmark_url
  type: string
- description: List of tools available on this project
  name: dock
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/project-schema.json
slug: project
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Project
---
