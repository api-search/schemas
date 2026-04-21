---
description: ApiVersion schema from APIs.guru REST API
layout: schema
name: ApiVersion
properties_list:
- description: Timestamp when the version was added
  name: added
  type: string
- description: Copy of `externalDocs` section from OpenAPI definition
  name: externalDocs
  type: object
- description: Copy of `info` section from OpenAPI definition
  name: info
  type: object
- description: Link to the individual API entry for this API
  name: link
  type: string
- description: The value of the `openapi` or `swagger` property of the source definition
  name: openapiVer
  type: string
- description: URL to OpenAPI definition in JSON format
  name: swaggerUrl
  type: string
- description: URL to OpenAPI definition in YAML format
  name: swaggerYamlUrl
  type: string
- description: Timestamp when the version was updated
  name: updated
  type: string
provider_name: APIs.guru
provider_slug: apis-guru
schema_file: json-schema/apis-guru-api-version-schema.json
slug: apis-guru-api-version
tags:
- API Catalog
- API Directory
- API Discovery
- Community
- GraphQL
- Open Source
- OpenAPI
title: ApiVersion
---
