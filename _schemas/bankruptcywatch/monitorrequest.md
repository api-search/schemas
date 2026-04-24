---
description: Bankruptcy monitoring request
layout: schema
name: MonitorRequest
properties_list:
- description: Monitor type (debtor, entity, portfolio)
  name: monitorType
  type: string
- description: Search criteria for triggering alerts
  name: criteria
  type: object
- description: ''
  name: notificationEmail
  type: string
- description: ''
  name: webhookUrl
  type: string
- description: ''
  name: label
  type: string
provider_name: BankruptcyWatch
provider_slug: bankruptcywatch
schema_file: json-schema/monitorrequest-schema.json
slug: monitorrequest
tags:
- Bankruptcy
- Compliance
- Court Data
- Legal
- Lending
- PACER
title: MonitorRequest
---
