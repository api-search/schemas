---
description: Equipment record returned by the CNH FieldOps API for agronomic and construction machinery (Case IH, New Holland, STEYR, Case CE, New Holland Construction).
layout: schema
name: CNH FieldOps Equipment
properties_list:
- description: FieldOps-assigned unique identifier for the vehicle.
  name: vehicleId
  type: string
- description: CNH Industrial brand.
  name: brand
  type: string
- description: Model name as registered with FieldOps.
  name: model
  type: string
- description: Manufacturer serial number / VIN-equivalent.
  name: serialNumber
  type: string
- description: Model year.
  name: year
  type: integer
- description: Vehicle category.
  name: vehicleType
  type: string
- description: Friendly display name set by the operator.
  name: displayName
  type: string
provider_name: CNH
provider_slug: cnh
schema_file: json-schema/cnh-equipment-schema.json
slug: cnh-equipment
tags:
- Agriculture
- Construction
- Telematics
- Equipment
- FieldOps
title: CNH FieldOps Equipment
---
