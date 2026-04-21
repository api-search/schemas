---
description: A purchase requisition with asset line items.
layout: schema
name: Requisition
properties_list:
- description: Requisition identifier.
  name: id
  type: string
- description: Requisition title or description.
  name: title
  type: string
- description: Current status of the requisition.
  name: status
  type: string
- description: Date and time the requisition was created.
  name: createdDate
  type: string
- description: Date and time the requisition was last updated.
  name: updatedDate
  type: string
- description: Line items in the requisition.
  name: lineItems
  type: array
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schema_file: json-schema/asset-management-api-requisition-schema.json
slug: asset-management-api-requisition
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
title: Requisition
---
