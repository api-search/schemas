---
description: An industrial asset monitored by Baker Hughes Cordant platform.
layout: schema
name: Asset
properties_list:
- description: Unique identifier for the asset.
  name: assetId
  type: string
- description: Human-readable name for the asset.
  name: assetName
  type: string
- description: Classification of the asset (e.g., compressor, pump, turbine).
  name: assetType
  type: string
- description: Identifier of the facility where the asset is located.
  name: facilityId
  type: string
- description: Geographic or plant location of the asset.
  name: location
  type: string
- description: Current operational status of the asset.
  name: status
  type: string
- description: AI-computed health score from 0 (critical) to 100 (healthy).
  name: healthScore
  type: number
- description: Timestamp of the last data update for this asset.
  name: lastUpdated
  type: string
- description: User-defined tags for organizing and filtering assets.
  name: tags
  type: array
provider_name: Baker Hughes
provider_slug: baker-hughes
schema_file: json-schema/baker-hughes-asset-schema.json
slug: baker-hughes-asset
tags:
- Energy Technology
- Industrial IoT
- Oil And Gas
- Asset Performance Management
- Digital Energy
title: Asset
---
