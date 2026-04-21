---
description: HTTP request configuration for Apache HttpComponents client
layout: schema
name: HttpRequest
properties_list:
- description: HTTP method
  name: method
  type: string
- description: Request URI
  name: uri
  type: string
- description: Request headers as key-value pairs
  name: headers
  type: object
- description: Request body content
  name: body
  type: string
- description: Content-Type header value
  name: contentType
  type: string
provider_name: Apache HttpComponents
provider_slug: apache-http
schema_file: json-schema/http-client-httprequest-schema.json
slug: http-client-httprequest
tags:
- Apache
- HTTP Client
- Java
- Open Source
- SDK
title: HttpRequest
---
