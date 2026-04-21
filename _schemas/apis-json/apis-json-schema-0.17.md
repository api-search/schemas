---
description: ''
layout: schema
name: A JSON Schema for apis.json, version 0.17
properties_list:
- description: The type of the APIs.json collection.
  name: type
  type: string
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
- description: APIs.json spec version, latest is 0.17
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
- description: Links to other apis.json definitions included in this service
  name: include
  type: array
- description: Common properties that apply across all APIs.
  name: common
  type: array
- description: Links to other apis.json that will be overlaid original.
  name: overlays
  type: array
provider_name: APIs.json
provider_slug: apis-json
schema_file: json-schema/apis-json-schema-0.17.json
slug: apis-json-schema-0.17
tags:
- API Aggregation
- API Cataloging
- API Commons
- API Discovery
- API Governance
- API Operations
- Machine Readable
- Specification
- Standard
title: A JSON Schema for apis.json, version 0.17
---
