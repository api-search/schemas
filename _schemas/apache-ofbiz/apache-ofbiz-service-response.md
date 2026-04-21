---
description: Standard API response from an OFBiz service invocation.
layout: schema
name: ServiceResponse
properties_list:
- description: HTTP status code.
  name: statusCode
  type: integer
- description: Human-readable status description.
  name: statusDescription
  type: string
- description: Success message if applicable.
  name: successMessage
  type: string
- description: Service output data. Structure varies by service.
  name: data
  type: object
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-service-response-schema.json
slug: apache-ofbiz-service-response
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: ServiceResponse
---
