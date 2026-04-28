---
description: Schema representing an agricultural field in the Climate FieldView platform, including its boundary, metadata, and associated agronomic layers.
layout: schema
name: Climate FieldView Field
properties_list:
- description: Unique field identifier
  name: id
  type: string
- description: Field name as entered by the grower
  name: name
  type: string
- description: Name of the grower who owns this field
  name: growerName
  type: string
- description: Farm or operation name the field belongs to
  name: farmName
  type: string
- description: Field area in acres
  name: acreage
  type: number
- description: Field boundary as a GeoJSON polygon
  name: boundary
  type: object
- description: Geographic centroid of the field
  name: centroid
  type: object
- description: US state abbreviation where the field is located
  name: state
  type: string
- description: County name where the field is located
  name: county
  type: string
- description: Field creation timestamp in the platform
  name: createdAt
  type: string
- description: Last field modification timestamp
  name: updatedAt
  type: string
provider_name: Climate FieldView
provider_slug: climate-fieldview
schema_file: json-schema/climate-fieldview-field-schema.json
slug: climate-fieldview-field
tags:
- Agriculture
- Bayer
- Crop Data
- Field Boundaries
- Harvest
- OAuth2
- Planting
- Precision Ag
title: Climate FieldView Field
---
