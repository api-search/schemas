---
description: List of basic metrics
layout: schema
name: Metrics
properties_list:
- description: Data used for charting etc
  name: datasets
  type: array
- description: Percentage of all APIs where auto fixes have been applied
  name: fixedPct
  type: integer
- description: Total number of fixes applied across all APIs
  name: fixes
  type: integer
- description: Number of newly invalid APIs
  name: invalid
  type: integer
- description: Open GitHub issues on our main repo
  name: issues
  type: integer
- description: Number of unique APIs
  name: numAPIs
  type: integer
- description: Number of methods of API retrieval
  name: numDrivers
  type: integer
- description: Total number of endpoints inside all definitions
  name: numEndpoints
  type: integer
- description: Number of API providers in directory
  name: numProviders
  type: integer
- description: Number of API definitions including different versions of the same API
  name: numSpecs
  type: integer
- description: GitHub stars for our main repo
  name: stars
  type: integer
- description: Summary totals for the last 7 days
  name: thisWeek
  type: object
- description: Number of unofficial APIs
  name: unofficial
  type: integer
- description: Number of unreachable (4XX,5XX status) APIs
  name: unreachable
  type: integer
provider_name: APIs.guru
provider_slug: apis-guru
schema_file: json-schema/apis-guru-metrics-schema.json
slug: apis-guru-metrics
tags:
- API Catalog
- API Directory
- API Discovery
- Community
- GraphQL
- Open Source
- OpenAPI
title: Metrics
---
