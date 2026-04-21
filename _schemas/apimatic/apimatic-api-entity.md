---
description: Schema representing an API entity (API definition) managed in the APIMatic platform
layout: schema
name: APIMatic API Entity
properties_list:
- description: Unique identifier of the API entity
  name: id
  type: string
- description: Name of the API
  name: name
  type: string
- description: Description of the API
  name: description
  type: string
- description: API version string
  name: version
  type: string
- description: Timestamp when the API entity was created
  name: createdAt
  type: string
- description: Timestamp when the API entity was last updated
  name: updatedAt
  type: string
provider_name: APIMatic
provider_slug: apimatic
schema_file: json-schema/apimatic-api-entity-schema.json
slug: apimatic-api-entity
tags:
- API Transformation
- Code Generation
- Developer Experience
- Documentation
- SDK Generation
title: APIMatic API Entity
---
