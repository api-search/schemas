---
description: A trade or shipping document managed within the CargoDocs platform, such as a bill of lading, certificate of origin, or invoice.
layout: schema
name: CargoDocs Document
properties_list:
- description: The unique identifier for the document.
  name: documentId
  type: string
- description: The type of document (e.g., eBoL, SWB, certificate, invoice).
  name: documentType
  type: string
- description: The current status of the document.
  name: status
  type: string
- description: The timestamp when the document was created.
  name: createdAt
  type: string
provider_name: CargoDocs
provider_slug: cargodocs
schema_file: json-schema/cargodocs-document.json
slug: cargodocs-document
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
title: CargoDocs Document
---
