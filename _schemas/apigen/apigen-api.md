---
description: An API definition within a project, including its generation source and lifecycle status.
layout: schema
name: APIGen API
properties_list:
- description: Unique identifier for the API.
  name: id
  type: string
- description: ID of the parent project.
  name: projectId
  type: string
- description: Human-readable name of the API.
  name: name
  type: string
- description: Detailed description of what the API does.
  name: description
  type: string
- description: Semantic version of the API.
  name: version
  type: string
- description: 'How the API was created: from a natural language prompt, an imported spec, or manually.'
  name: generationSource
  type: string
- description: The natural language prompt used to generate the API, if applicable.
  name: prompt
  type: string
- description: URL to the imported OpenAPI specification, if applicable.
  name: specUrl
  type: string
- description: Current lifecycle status of the API.
  name: status
  type: string
- description: Number of endpoints defined in this API.
  name: endpointCount
  type: integer
- description: Number of schemas defined in this API.
  name: schemaCount
  type: integer
- description: Tags for categorizing the API.
  name: tags
  type: array
- description: Timestamp when the API was created.
  name: createdAt
  type: string
- description: Timestamp when the API was last updated.
  name: updatedAt
  type: string
provider_name: APIGen
provider_slug: apigen
schema_file: json-schema/apigen-api-schema.json
slug: apigen-api
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
title: APIGen API
---
