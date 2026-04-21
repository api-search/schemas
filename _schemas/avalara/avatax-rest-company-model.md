---
description: CompanyModel schema from Avalara API
layout: schema
name: CompanyModel
properties_list:
- description: Unique identifier for the company
  name: id
  type: integer
- description: Short code identifying this company
  name: companyCode
  type: string
- description: Display name of the company
  name: name
  type: string
- description: Whether this is the default company for the account
  name: isDefault
  type: boolean
- description: ''
  name: isActive
  type: boolean
- description: Tax identification number (EIN, TIN)
  name: taxpayerIdNumber
  type: string
- description: ''
  name: hasProfile
  type: boolean
- description: ''
  name: isReportingEntity
  type: boolean
- description: Default country for this company
  name: defaultCountry
  type: string
- description: Default currency code
  name: baseCurrencyCode
  type: string
- description: ''
  name: sstEffDate
  type: string
- description: ''
  name: roundingLevelId
  type: string
- description: ''
  name: sstPId
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-company-model-schema.json
slug: avatax-rest-company-model
tags:
- Taxes
title: CompanyModel
---
