---
description: An API specification within an API Fiddle project, representing an OpenAPI document being designed or edited.
layout: schema
name: API Fiddle Specification
properties_list:
- description: Unique identifier for the specification.
  name: id
  type: string
- description: Identifier of the parent project.
  name: projectId
  type: string
- description: Name of the specification.
  name: name
  type: string
- description: A detailed description of the specification.
  name: description
  type: string
- description: Version label for the specification.
  name: version
  type: string
- description: The OpenAPI format version used by this specification.
  name: format
  type: string
- description: The raw specification content in YAML or JSON.
  name: content
  type: string
- description: Current lifecycle status of the specification.
  name: status
  type: string
- description: Timestamp when the specification was created.
  name: createdAt
  type: string
- description: Timestamp when the specification was last updated.
  name: updatedAt
  type: string
provider_name: API-Fiddle
provider_slug: api-fiddle
schema_file: json-schema/api-fiddle-specification-schema.json
slug: api-fiddle-specification
tags:
- API Design
- OpenAPI
- Collaboration
- Documentation
- Platform
title: API Fiddle Specification
---
