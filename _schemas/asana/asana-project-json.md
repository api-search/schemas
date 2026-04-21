---
description: A project represents a prioritized list of tasks in Asana or a board with columns of tasks represented as cards. It exists in a single workspace or organization.
layout: schema
name: Asana Project
properties_list:
- description: Globally unique identifier of the resource.
  name: gid
  type: string
- description: The base type of this resource.
  name: resource_type
  type: string
- description: Name of the project.
  name: name
  type: string
- description: True if the project is archived.
  name: archived
  type: boolean
- description: Color of the project.
  name: color
  type:
  - string
  - 'null'
- description: The time at which this resource was created.
  name: created_at
  type: string
- description: The time at which this project was last modified.
  name: modified_at
  type: string
- description: The day on which this project is due (YYYY-MM-DD).
  name: due_on
  type:
  - string
  - 'null'
- description: The day on which work begins for this project (YYYY-MM-DD).
  name: start_on
  type:
  - string
  - 'null'
- description: The default view of a project.
  name: default_view
  type: string
- description: Free-form textual information associated with the project.
  name: notes
  type: string
- description: The notes of the project with formatting as HTML.
  name: html_notes
  type: string
- description: The privacy setting of the project.
  name: privacy_setting
  type: string
- description: The default access for users or teams who join the project.
  name: default_access_level
  type: string
- description: True if the project is currently marked complete.
  name: completed
  type: boolean
- description: The time at which this project was completed.
  name: completed_at
  type:
  - string
  - 'null'
- description: The current owner of the project.
  name: owner
  type: object
- description: The team that this project is shared with.
  name: team
  type: object
- description: The workspace or organization this project is associated with.
  name: workspace
  type: object
- description: Array of users who are members of this project.
  name: members
  type: array
- description: Array of users following this project.
  name: followers
  type: array
- description: The icon for a project.
  name: icon
  type:
  - string
  - 'null'
- description: A URL that points directly to the object within Asana.
  name: permalink_url
  type: string
provider_name: Asana
provider_slug: asana
schema_file: json-schema/asana-project-json-schema.json
slug: asana-project-json
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
title: Asana Project
---
