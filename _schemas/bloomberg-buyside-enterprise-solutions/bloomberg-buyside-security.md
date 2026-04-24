---
description: A financial security representing an instrument in Bloomberg's data universe, including equities, fixed income, derivatives, funds, and other asset classes with reference data, identifiers, and classification information.
layout: schema
name: Bloomberg Buyside Security
properties_list:
- description: Bloomberg ticker symbol (e.g., 'AAPL US Equity')
  name: ticker
  type: string
- description: Full security name
  name: name
  type: string
- description: Abbreviated security name
  name: shortName
  type: string
- description: Primary asset class classification
  name: assetClass
  type: string
- description: Specific security type within the asset class
  name: securityType
  type: string
- description: Primary exchange where the security is listed
  name: exchange
  type: string
- description: Country of domicile (ISO 3166-1 alpha-2)
  name: country
  type: string
- description: Trading currency (ISO 4217)
  name: currency
  type: string
- description: ''
  name: identifiers
  type: object
- description: ''
  name: classification
  type: object
- description: Issuer name
  name: issuer
  type: string
- description: Original issue date
  name: issueDate
  type: string
- description: Maturity date (for fixed income and derivatives)
  name: maturityDate
  type: string
- description: Coupon rate for fixed income securities
  name: couponRate
  type: number
- description: Coupon payment frequency
  name: couponFrequency
  type: string
- description: Par or face value
  name: parAmount
  type: number
- description: Market capitalization (for equities)
  name: marketCap
  type: number
- description: Total shares outstanding (for equities)
  name: sharesOutstanding
  type: number
- description: Indicated dividend yield
  name: dividendYield
  type: number
- description: ''
  name: rating
  type: object
- description: Whether the security is currently active and trading
  name: active
  type: boolean
provider_name: Bloomberg Buyside Enterprise Solutions
provider_slug: bloomberg-buyside-enterprise-solutions
schema_file: json-schema/bloomberg-buyside-security-schema.json
slug: bloomberg-buyside-security
tags:
- Analytics
- Asset Management
- Buy-Side
- Enterprise Solutions
- Financial Services
- Market Data
- Portfolio Management
- Trading
title: Bloomberg Buyside Security
---
