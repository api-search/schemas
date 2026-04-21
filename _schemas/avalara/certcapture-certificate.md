---
description: Certificate schema from Avalara API
layout: schema
name: Certificate
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: certificateNumber
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: signedDate
  type: string
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: exemptionNumber
  type: string
- description: ''
  name: exemptionReason
  type: string
- description: ''
  name: exemptPercentage
  type: number
- description: Jurisdiction where the exemption applies
  name: exposureZone
  type: string
- description: ''
  name: customer
  type: object
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/certcapture-certificate-schema.json
slug: certcapture-certificate
tags:
- Taxes
title: Certificate
---
