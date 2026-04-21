---
description: APIsJSON schema from APIs.io Search API
layout: schema
name: APIsJSON
properties_list:
- description: The name of the service described
  name: name
  type: string
- description: Description of the service
  name: description
  type: string
- description: URL where the apis.json file will live
  name: url
  type: string
- description: Image to represent the API
  name: image
  type: string
- description: Date when the file was created
  name: created
  type: string
- description: Date when the file was modified
  name: modified
  type: string
- description: APIs.json spec version, latest is 0.18
  name: specificationVersion
  type: string
- description: All the APIs of this service
  name: apis
  type: array
- description: Maintainers of the apis.json file
  name: maintainers
  type: array
- description: Tags to describe the service
  name: tags
  type: array
- description: Links to other apis.json definitions included in this service.
  name: include
  type: array
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-ap-is-json-schema.json
slug: apis-io-search-ap-is-json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: APIsJSON
---
