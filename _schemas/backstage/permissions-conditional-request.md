---
description: ConditionalRequest schema from Backstage permissions API
layout: schema
name: ConditionalRequest
properties_list:
- description: Reference to the resource.
  name: resourceRef
  type: string
- description: The resource type identifier.
  name: resourceType
  type: string
- description: The conditions to evaluate against the resource.
  name: conditions
  type: object
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/permissions-conditional-request-schema.json
slug: permissions-conditional-request
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: ConditionalRequest
---
