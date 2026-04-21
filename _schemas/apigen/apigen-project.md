---
description: An API generation project that groups related APIs, connectors, and configurations.
layout: schema
name: APIGen Project
properties_list:
- description: Unique identifier for the project.
  name: id
  type: string
- description: Human-readable name of the project.
  name: name
  type: string
- description: Detailed description of the project purpose and scope.
  name: description
  type: string
- description: Current lifecycle status of the project.
  name: status
  type: string
- description: User ID of the project owner.
  name: ownerId
  type: string
- description: Project-level settings and preferences.
  name: settings
  type: object
- description: Tags for categorizing the project.
  name: tags
  type: array
- description: Timestamp when the project was created.
  name: createdAt
  type: string
- description: Timestamp when the project was last updated.
  name: updatedAt
  type: string
provider_name: APIGen
provider_slug: apigen
schema_file: json-schema/apigen-project-schema.json
slug: apigen-project
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
title: APIGen Project
---
