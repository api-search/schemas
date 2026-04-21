---
description: A user object represents an account in Asana that can be given access to various workspaces, projects, and tasks. The special string identifier 'me' can be used to refer to the current authenticated user.
layout: schema
name: Asana User
properties_list:
- description: Globally unique identifier of the resource.
  name: gid
  type: string
- description: The base type of this resource.
  name: resource_type
  type: string
- description: The user's name. Read-only except when same user as requester.
  name: name
  type: string
- description: The user's email address.
  name: email
  type: string
- description: A map of the user's profile photo in various sizes.
  name: photo
  type:
  - object
  - 'null'
- description: Workspaces and organizations this user may access.
  name: workspaces
  type: array
provider_name: Asana
provider_slug: asana
schema_file: json-schema/asana-user-json-schema.json
slug: asana-user-json
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
title: Asana User
---
