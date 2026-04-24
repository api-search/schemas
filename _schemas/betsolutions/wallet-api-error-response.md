---
description: Error response returned when a request fails.
layout: schema
name: ErrorResponse
properties_list:
- description: Always false for error responses.
  name: success
  type: boolean
- description: Numeric error code.
  name: errorCode
  type: integer
- description: Human-readable error description.
  name: errorMessage
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-error-response-schema.json
slug: wallet-api-error-response
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: ErrorResponse
---
