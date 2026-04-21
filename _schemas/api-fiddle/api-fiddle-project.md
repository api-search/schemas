---
description: An API design project within the API Fiddle platform containing one or more API specifications.
layout: schema
name: API Fiddle Project
properties_list:
- description: Unique identifier for the project.
  name: id
  type: string
- description: Name of the project.
  name: name
  type: string
- description: A detailed description of the project.
  name: description
  type: string
- description: Identifier of the workspace this project belongs to.
  name: workspaceId
  type: string
- description: Visibility level of the project.
  name: visibility
  type: string
- description: List of specifications associated with this project.
  name: specifications
  type: array
- description: Tags for categorizing the project.
  name: tags
  type: array
- description: Timestamp when the project was created.
  name: createdAt
  type: string
- description: Timestamp when the project was last updated.
  name: updatedAt
  type: string
provider_name: API-Fiddle
provider_slug: api-fiddle
schema_file: json-schema/api-fiddle-project-schema.json
slug: api-fiddle-project
tags:
- API Design
- OpenAPI
- Collaboration
- Documentation
- Platform
title: API Fiddle Project
---
