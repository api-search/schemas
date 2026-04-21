---
description: HTTP response from Apache HttpComponents client execution
layout: schema
name: HttpResponse
properties_list:
- description: HTTP response status code
  name: statusCode
  type: integer
- description: HTTP reason phrase
  name: reasonPhrase
  type: string
- description: Response headers as key-value pairs
  name: headers
  type: object
- description: Response body content
  name: body
  type: string
- description: Content-Type of the response body
  name: contentType
  type: string
provider_name: Apache HttpComponents
provider_slug: apache-http
schema_file: json-schema/http-client-httpresponse-schema.json
slug: http-client-httpresponse
tags:
- Apache
- HTTP Client
- Java
- Open Source
- SDK
title: HttpResponse
---
