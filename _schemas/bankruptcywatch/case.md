---
description: A US bankruptcy court case
layout: schema
name: Case
properties_list:
- description: BankruptcyWatch internal case ID
  name: caseId
  type: string
- description: PACER case number
  name: caseNumber
  type: string
- description: Name of the debtor
  name: debtorName
  type: string
- description: Bankruptcy chapter (7, 11, 13, etc.)
  name: chapter
  type: string
- description: Bankruptcy court district code
  name: district
  type: string
- description: Date the case was filed
  name: dateFiled
  type: string
- description: Current case status
  name: status
  type: string
- description: Assigned bankruptcy judge
  name: judge
  type: string
- description: Appointed trustee name
  name: trustee
  type: string
- description: Asset amount range
  name: assets
  type: string
- description: Liability amount range
  name: liabilities
  type: string
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/case-schema.json
slug: case
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: Case
---
