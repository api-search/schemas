---
description: Payment beneficiary details
layout: schema
name: Beneficiary
properties_list:
- description: Beneficiary name
  name: name
  type: string
- description: Beneficiary account number
  name: accountNumber
  type: string
- description: Beneficiary bank routing number (ABA)
  name: routingNumber
  type: string
- description: Beneficiary bank name
  name: bankName
  type: string
- description: Beneficiary bank address
  name: bankAddress
  type: string
- description: SWIFT/BIC code for international wires
  name: swiftCode
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/beneficiary-schema.json
slug: beneficiary
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Beneficiary
---
