---
description: An asset line item on a requisition.
layout: schema
name: AssetLineItem
properties_list:
- description: Line item identifier.
  name: lineItemId
  type: string
- description: Line item description.
  name: description
  type: string
- description: Asset category classification.
  name: assetCategory
  type: string
- description: Quantity ordered.
  name: quantity
  type: integer
- description: Assigned asset number (populated after update).
  name: assetNumber
  type: string
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-asset-line-item-schema.json
slug: asset-management-api-asset-line-item
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: AssetLineItem
---
