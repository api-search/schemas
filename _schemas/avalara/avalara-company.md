---
description: A company represents a legal entity within AvaTax that can calculate and report taxes. Companies contain locations, nexus declarations, items, and other tax configuration data.
layout: schema
name: Avalara Company
properties_list:
- description: Unique identifier for the company
  name: id
  type: integer
- description: Short code identifying this company in transactions
  name: companyCode
  type: string
- description: Display name of the company
  name: name
  type: string
- description: Account ID that owns this company
  name: accountId
  type: integer
- description: Parent company ID for multi-company hierarchies
  name: parentCompanyId
  type: integer
- description: Whether this is the default company for the account
  name: isDefault
  type: boolean
- description: Whether the company is currently active
  name: isActive
  type: boolean
- description: Tax identification number (EIN, TIN, VAT number)
  name: taxpayerIdNumber
  type: string
- description: Whether the company has a completed tax profile
  name: hasProfile
  type: boolean
- description: Whether this company is a reporting entity
  name: isReportingEntity
  type: boolean
- description: Two-character ISO 3166 country code for the default country
  name: defaultCountry
  type: string
- description: Three-character ISO 4217 currency code
  name: baseCurrencyCode
  type: string
- description: Level at which tax rounding is applied
  name: roundingLevelId
  type: string
- description: ''
  name: address
  type: object
- description: Nexus declarations for this company
  name: nexus
  type: array
- description: Physical locations belonging to this company
  name: locations
  type: array
- description: Date and time the company was created
  name: createdDate
  type: string
- description: Date and time the company was last modified
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avalara-company-schema.json
slug: avalara-company
tags:
- Taxes
title: Avalara Company
---
