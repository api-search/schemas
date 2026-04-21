---
description: Schema representing an API registered in the Apinity compliant API marketplace
layout: schema
name: Apinity Marketplace API
properties_list:
- description: Unique identifier for the marketplace API
  name: id
  type: string
- description: Name of the API
  name: name
  type: string
- description: Description of the API and its capabilities
  name: description
  type: string
- description: Organization providing the API
  name: provider
  type: string
- description: API version
  name: version
  type: string
- description: Lifecycle status of the API in the marketplace
  name: status
  type: string
- description: Compliance policies applied to this API
  name: compliancePolicies
  type: array
- description: Categories classifying this API in the marketplace
  name: categories
  type: array
- description: Timestamp when the API was registered in the marketplace
  name: createdAt
  type: string
provider_name: Apinity.io
provider_slug: apinity-io
schema_file: json-schema/apinity-marketplace-schema.json
slug: apinity-marketplace
tags:
- API Governance
- API Marketplace
- Compliance
- Discovery
- Integration Platform
title: Apinity Marketplace API
---
