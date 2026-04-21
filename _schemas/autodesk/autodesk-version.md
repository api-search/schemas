---
description: A version represents a specific revision of an item in the Autodesk Data Management system. Each time a file is uploaded or modified, a new version is created, enabling version history tracking and rollback capabilities.
layout: schema
name: Autodesk Version
properties_list:
- description: The JSON:API resource type.
  name: type
  type: string
- description: The unique version identifier (URN).
  name: id
  type: string
- description: ''
  name: attributes
  type: object
- description: ''
  name: relationships
  type: object
provider_name: Autodesk
provider_slug: autodesk
schema_file: json-schema/autodesk-version.json
slug: autodesk-version
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
title: Autodesk Version
---
