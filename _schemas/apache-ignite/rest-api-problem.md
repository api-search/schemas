---
description: Extended description of the problem with the request.
layout: schema
name: Problem
properties_list:
- description: Short summary of the issue.
  name: title
  type: string
- description: Returned HTTP status code.
  name: status
  type: integer
- description: Ignite 3 error code.
  name: code
  type: string
- description: URI to documentation regarding the issue.
  name: type
  type: string
- description: Extended explanation of the issue.
  name: detail
  type: string
- description: Name of the node the issue happened on.
  name: node
  type: string
- description: Unique issue identifier. This identifier can be used to find logs related to the issue.
  name: traceId
  type: string
- description: A list of parameters that did not pass validation and the reason for it.
  name: invalidParams
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-problem-schema.json
slug: rest-api-problem
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: Problem
---
