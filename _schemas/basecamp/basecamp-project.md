---
description: Represents a Basecamp project (bucket), which is the top-level container for all collaboration content including messages, to-dos, documents, schedules, campfires, and card tables. Projects are owned by an account and can be accessed by invited team members and clients.
layout: schema
name: Basecamp Project
properties_list:
- description: Unique identifier for the project within the Basecamp account
  name: id
  type: integer
- description: Current lifecycle status of the project
  name: status
  type: string
- description: ISO 8601 UTC timestamp when the project was created
  name: created_at
  type: string
- description: ISO 8601 UTC timestamp when the project was last updated
  name: updated_at
  type: string
- description: Human-readable name of the project
  name: name
  type: string
- description: Optional description providing context about the project's purpose or scope
  name: description
  type:
  - string
  - 'null'
- description: Project purpose classification such as 'team_project' or 'company_hq'
  name: purpose
  type: string
- description: Whether client visibility is enabled for this project, allowing invited client users to view designated content
  name: clients_enabled
  type: boolean
- description: Whether timesheet tracking is enabled for this project
  name: timesheet_enabled
  type: boolean
- description: Optional color identifier used to visually distinguish the project in the Basecamp interface
  name: color
  type:
  - string
  - 'null'
- description: Canonical API URL for this project resource
  name: url
  type: string
- description: Web URL to open this project in the Basecamp application
  name: app_url
  type: string
- description: API URL to bookmark this project for the authenticated user
  name: bookmark_url
  type: string
- description: List of tools available on this project's dock, each representing an enabled feature such as messages, to-dos, schedule, or campfire
  name: dock
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/basecamp-project-schema.json
slug: basecamp-project
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Basecamp Project
---
