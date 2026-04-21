---
description: An API endpoint defining a single operation with its path, method, and request/response schemas.
layout: schema
name: APIGen Endpoint
properties_list:
- description: Unique identifier for the endpoint.
  name: id
  type: string
- description: ID of the parent API.
  name: apiId
  type: string
- description: URL path for the endpoint, starting with a forward slash.
  name: path
  type: string
- description: HTTP method for the endpoint.
  name: method
  type: string
- description: Short summary of what the endpoint does.
  name: summary
  type: string
- description: Detailed description of the endpoint behavior.
  name: description
  type: string
- description: Path, query, and header parameters.
  name: parameters
  type: array
- description: JSON Schema defining the request body.
  name: requestSchema
  type: object
- description: JSON Schema defining the success response body.
  name: responseSchema
  type: object
- description: Whether this endpoint requires authentication.
  name: authentication
  type: boolean
- description: ID of the connector used as the data source for this endpoint.
  name: connectorId
  type:
  - string
  - 'null'
- description: Timestamp when the endpoint was created.
  name: createdAt
  type: string
- description: Timestamp when the endpoint was last updated.
  name: updatedAt
  type: string
provider_name: APIGen
provider_slug: apigen
schema_file: json-schema/apigen-endpoint-schema.json
slug: apigen-endpoint
tags:
- Code
- Documentation
- Generation
- Open Source
- PHP
title: APIGen Endpoint
---
