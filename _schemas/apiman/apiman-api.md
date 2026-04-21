---
description: Schema representing an API managed by the Apiman API management platform
layout: schema
name: Apiman API
properties_list:
- description: Organization identifier owning this API
  name: organizationId
  type: string
- description: Unique identifier for the API
  name: id
  type: string
- description: Name of the API
  name: name
  type: string
- description: Description of the API
  name: description
  type: string
- description: Username of the user who created the API
  name: createdBy
  type: string
- description: Timestamp when the API was created
  name: createdOn
  type: string
- description: Number of published versions of this API
  name: numPublished
  type: integer
- description: Tags associated with the API
  name: tags
  type: array
provider_name: Apiman
provider_slug: apiman
schema_file: json-schema/apiman-api-schema.json
slug: apiman-api
tags:
- API Gateway
- API Management
- Developer Portal
- Java
- Open Source
title: Apiman API
---
