---
description: A workspace within the API Fiddle platform used to organize and group related API design projects.
layout: schema
name: API Fiddle Workspace
properties_list:
- description: Unique identifier for the workspace.
  name: id
  type: string
- description: Name of the workspace.
  name: name
  type: string
- description: A detailed description of the workspace.
  name: description
  type: string
- description: Identifier of the user who owns the workspace.
  name: ownerId
  type: string
- description: List of members with access to the workspace.
  name: members
  type: array
- description: List of project identifiers within this workspace.
  name: projects
  type: array
- description: Timestamp when the workspace was created.
  name: createdAt
  type: string
- description: Timestamp when the workspace was last updated.
  name: updatedAt
  type: string
provider_name: API-Fiddle
provider_slug: api-fiddle
schema_file: json-schema/api-fiddle-workspace-schema.json
slug: api-fiddle-workspace
tags:
- API Design
- OpenAPI
- Collaboration
- Documentation
- Platform
title: API Fiddle Workspace
---
