---
description: ''
layout: schema
name: SafetyInfo
properties_list:
- description: Country slug
  name: country
  type: string
- description: ''
  name: overallRating
  type: string
- description: Advisory level (1=normal, 4=do not travel)
  name: advisoryLevel
  type: integer
- description: ''
  name: categories
  type: object
- description: Additional safety notes
  name: notes
  type: string
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/safetyinfo.json
slug: safetyinfo
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: SafetyInfo
---
