---
description: Represents an Apidog project, the top-level container for endpoints, schemas, and environments managed through the Apidog API.
layout: schema
name: Apidog Project
properties_list:
- description: The unique identifier of the Apidog project.
  name: projectId
  type: integer
- description: The human-readable name of the project.
  name: name
  type: string
- description: A brief description of what this project contains.
  name: description
  type: string
- description: Total number of API endpoints in the project.
  name: endpointCount
  type: integer
- description: Total number of data schemas in the project.
  name: schemaCount
  type: integer
- description: Total number of environments configured in the project.
  name: environmentCount
  type: integer
- description: The Apidog API version used when interacting with this project.
  name: apiVersion
  type: string
provider_name: Apidog
provider_slug: apidog
schema_file: json-schema/apidog-project-schema.json
slug: apidog-project
tags:
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- Mocking
- Platform
title: Apidog Project
---
