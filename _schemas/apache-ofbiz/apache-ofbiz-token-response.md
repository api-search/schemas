---
description: Standard API response containing JWT token data.
layout: schema
name: TokenResponse
properties_list:
- description: HTTP status code.
  name: statusCode
  type: integer
- description: Human-readable status description.
  name: statusDescription
  type: string
- description: Success message from the server.
  name: successMessage
  type: string
- description: JWT token data returned after successful authentication.
  name: data
  type: object
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-token-response-schema.json
slug: apache-ofbiz-token-response
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: TokenResponse
---
