---
description: API error response
layout: schema
name: ErrorResponse
properties_list:
- description: Machine-readable error code
  name: errorCode
  type: string
- description: Human-readable error message
  name: message
  type: string
- description: Additional error details
  name: details
  type: array
- description: Request identifier for support
  name: requestId
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/errorresponse-schema.json
slug: errorresponse
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: ErrorResponse
---
