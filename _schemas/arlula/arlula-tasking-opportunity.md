---
description: A future satellite capture opportunity.
layout: schema
name: TaskingOpportunity
properties_list:
- description: Ordering ID for this tasking opportunity.
  name: id
  type: string
- description: Supplier identifier.
  name: supplier
  type: string
- description: Earliest start time for the capture window.
  name: captureStart
  type: string
- description: Latest end time for the capture window.
  name: captureEnd
  type: string
- description: Expected ground sample distance in meters.
  name: gsd
  type: number
- description: Price for this tasking opportunity.
  name: price
  type: number
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-tasking-opportunity-schema.json
slug: arlula-tasking-opportunity
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: TaskingOpportunity
---
