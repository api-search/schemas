---
description: SimSwapCheckRequest schema
layout: schema
name: SimSwapCheckRequest
properties_list:
- description: Mobile phone number in E.164 format associated with the SIM to check.
  name: phoneNumber
  type: string
- description: Maximum age in hours to check for a SIM swap. If not provided, the default lookback period is used.
  name: maxAge
  type: integer
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/sim-swap-api-sim-swap-check-request-schema.json
slug: sim-swap-api-sim-swap-check-request
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: SimSwapCheckRequest
---
