---
description: An electronic bill of lading (eBoL) or sea waybill (SWB) managed through the CargoDocs platform, representing a document of title for shipped cargo.
layout: schema
name: CargoDocs Bill of Lading
properties_list:
- description: The unique identifier for the bill of lading document.
  name: documentId
  type: string
- description: The type of bill of lading document.
  name: documentType
  type: string
- description: The unique identifier for the transaction this bill of lading belongs to.
  name: transactionId
  type: string
- description: The current status of the bill of lading (e.g., draft, issued, surrendered).
  name: status
  type: string
- description: The unique identifier for the draft version of this bill of lading.
  name: draftId
  type: string
- description: Details of the shipper named on the bill of lading.
  name: shipperDetails
  type: object
- description: Details of the consignee named on the bill of lading.
  name: consigneeDetails
  type: object
- description: Details of the cargo described on the bill of lading.
  name: cargoDetails
  type: object
- description: The timestamp when the bill of lading was issued.
  name: issuedAt
  type: string
- description: The timestamp when the bill of lading was created.
  name: createdAt
  type: string
provider_name: CargoDocs
provider_slug: cargodocs
schema_file: json-schema/cargodocs-bill-of-lading.json
slug: cargodocs-bill-of-lading
tags:
- Bills of Lading
- Documentation
- eBoL
- EssDocs
- MLETR
- Shipping
- Supply Chain
- Trade
- Trade Finance
- Warehouse Warrants
title: CargoDocs Bill of Lading
---
