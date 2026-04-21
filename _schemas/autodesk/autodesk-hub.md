---
description: A hub represents an Autodesk account (such as BIM 360, ACC, or Fusion Team) that serves as the top-level container for projects and data. Hubs provide organizational context for all data management operations.
layout: schema
name: Autodesk Hub
properties_list:
- description: The JSON:API resource type.
  name: type
  type: string
- description: The unique hub identifier, prefixed with 'b.' for BIM 360/ACC or 'a.' for Autodesk accounts.
  name: id
  type: string
- description: ''
  name: attributes
  type: object
- description: ''
  name: relationships
  type: object
- description: ''
  name: links
  type: object
provider_name: Autodesk
provider_slug: autodesk
schema_file: json-schema/autodesk-hub.json
slug: autodesk-hub
tags:
- 3D Modeling
- Architecture
- BIM
- CAD
- Construction
- Design
- Digital Twins
- Engineering
- Manufacturing
- Media and Entertainment
- Sustainability
title: Autodesk Hub
---
