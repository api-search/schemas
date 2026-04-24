---
description: A transaction in the CargoDocs platform representing a trade or shipping workflow that groups related electronic documents together.
layout: schema
name: CargoDocs Transaction
properties_list:
- description: The unique identifier for the transaction.
  name: transactionId
  type: string
- description: The current status of the transaction.
  name: status
  type: string
- description: The timestamp when the transaction was created.
  name: createdAt
  type: string
- description: The number of documents associated with this transaction.
  name: documentCount
  type: integer
provider_name: CargoDocs
provider_slug: cargodocs
schema_file: json-schema/cargodocs-transaction.json
slug: cargodocs-transaction
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
title: CargoDocs Transaction
---
