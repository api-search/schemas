---
description: Schema representing an API available on the APILayer marketplace
layout: schema
name: APILayer API
properties_list:
- description: Unique identifier for the API
  name: id
  type: string
- description: Name of the API
  name: name
  type: string
- description: Description of the API and its capabilities
  name: description
  type: string
- description: Category of the API (e.g., Geolocation, Currency, Weather)
  name: category
  type: string
- description: Base URL for API requests
  name: baseURL
  type: string
- description: URL to the API documentation
  name: documentationURL
  type: string
- description: Authentication details for the API
  name: authentication
  type: object
- description: Available subscription plans for this API
  name: plans
  type: array
- description: Tags describing the API
  name: tags
  type: array
provider_name: APILayer
provider_slug: apilayer
schema_file: json-schema/apilayer-api-schema.json
slug: apilayer-api
tags:
- API Catalog
- API Discovery
- API Marketplace
- Developer Tools
- SaaS APIs
title: APILayer API
---
