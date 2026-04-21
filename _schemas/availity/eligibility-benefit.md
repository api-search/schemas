---
description: Benefit schema from Availity API
layout: schema
name: Benefit
properties_list:
- description: X12 benefit information code
  name: code
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: coverageLevel
  type: string
- description: ''
  name: benefitAmount
  type: object
- description: ''
  name: benefitPercent
  type: number
- description: ''
  name: inPlanNetworkIndicator
  type: string
- description: Benefit period (e.g., Calendar Year, Plan Year, Lifetime)
  name: timeQualifier
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/eligibility-benefit-schema.json
slug: eligibility-benefit
tags: []
title: Benefit
---
