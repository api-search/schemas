---
description: JSON Schema for an Availity healthcare eligibility and benefits response (equivalent to X12 271 transaction).
layout: schema
name: Availity Eligibility Response
properties_list:
- description: Availity transaction identifier
  name: id
  type: string
- description: Transaction control number matching the request
  name: controlNumber
  type: string
- description: ''
  name: requestedDate
  type: string
- description: ''
  name: serviceDate
  type: string
- description: ''
  name: subscriber
  type: object
- description: ''
  name: payer
  type: object
- description: ''
  name: coverages
  type: array
- description: ''
  name: planInformation
  type: object
provider_name: availity
provider_slug: availity
schema_file: json-schema/availity-eligibility-schema.json
slug: availity-eligibility
tags: []
title: Availity Eligibility Response
---
