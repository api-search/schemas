---
description: Semiconductor manufacturing equipment managed by Applied Materials
layout: schema
name: Equipment
properties_list:
- description: Unique equipment identifier
  name: equipmentId
  type: string
- description: Equipment serial number
  name: serialNumber
  type: string
- description: Equipment model name
  name: model
  type: string
- description: Equipment type (CVD, PVD, CMP, Etch, etc.)
  name: type
  type: string
- description: Current operational status
  name: status
  type: string
- description: Fab location where equipment is installed
  name: location
  type: string
- description: Date equipment was installed
  name: installDate
  type: string
- description: Date of last scheduled maintenance
  name: lastMaintenanceDate
  type: string
provider_name: Applied Materials
provider_slug: applied-materials
schema_file: json-schema/equipment-schema.json
slug: equipment
tags:
- Semiconductor
- Manufacturing
- Equipment
- Fab Operations
- Materials Engineering
title: Equipment
---
