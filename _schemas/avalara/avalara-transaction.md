---
description: A tax transaction represents a taxable event such as a sale, purchase, or return processed through the AvaTax API. It contains header-level information, line items, calculated tax amounts, and jurisdiction details.
layout: schema
name: Avalara Tax Transaction
properties_list:
- description: Unique identifier for the transaction
  name: id
  type: integer
- description: Unique transaction code assigned by the client or auto-generated
  name: code
  type: string
- description: Code identifying the company that owns this transaction
  name: companyCode
  type: string
- description: The document type for this transaction
  name: type
  type: string
- description: Current lifecycle status of the transaction
  name: status
  type: string
- description: Date of the transaction
  name: date
  type: string
- description: Unique code identifying the customer for this transaction
  name: customerCode
  type: string
- description: Three-character ISO 4217 currency code
  name: currencyCode
  type: string
- description: Whether the transaction should be committed immediately
  name: commit
  type: boolean
- description: Total amount of the transaction before tax
  name: totalAmount
  type: number
- description: Total tax calculated for the transaction
  name: totalTax
  type: number
- description: Total taxable amount
  name: totalTaxable
  type: number
- description: Total exempt amount
  name: totalExempt
  type: number
- description: Total discount applied
  name: totalDiscount
  type: number
- description: Total tax calculated before any adjustments
  name: totalTaxCalculated
  type: number
- description: Address information for the transaction
  name: addresses
  type: object
- description: Line items included in this transaction
  name: lines
  type: array
- description: Tax summary broken down by jurisdiction
  name: summary
  type: array
- description: Date and time the transaction was created
  name: createdDate
  type: string
- description: Date and time the transaction was last modified
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avalara-transaction-schema.json
slug: avalara-transaction
tags:
- Taxes
title: Avalara Tax Transaction
---
