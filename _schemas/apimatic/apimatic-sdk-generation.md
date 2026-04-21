---
description: Schema representing an SDK generation request and result in APIMatic
layout: schema
name: APIMatic SDK Generation
properties_list:
- description: Target SDK platform for code generation
  name: platform
  type: string
- description: URL to download the generated SDK package
  name: downloadUrl
  type: string
- description: Expiration timestamp for the download URL
  name: expiresAt
  type: string
provider_name: APIMatic
provider_slug: apimatic
schema_file: json-schema/apimatic-sdk-generation-schema.json
slug: apimatic-sdk-generation
tags:
- API Transformation
- Code Generation
- Developer Experience
- Documentation
- SDK Generation
title: APIMatic SDK Generation
---
