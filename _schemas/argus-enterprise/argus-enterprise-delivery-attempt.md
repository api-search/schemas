---
description: DeliveryAttempt schema from ARGUS Enterprise API
layout: schema
name: DeliveryAttempt
properties_list:
- description: Sequential attempt number
  name: attemptNumber
  type: integer
- description: When the delivery was attempted
  name: timestamp
  type: string
- description: HTTP response status code from the endpoint
  name: responseCode
  type: integer
- description: Response time in milliseconds
  name: responseTime
  type: integer
- description: Whether the delivery was successful
  name: success
  type: boolean
- description: Error message if delivery failed
  name: errorMessage
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-delivery-attempt-schema.json
slug: argus-enterprise-delivery-attempt
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: DeliveryAttempt
---
