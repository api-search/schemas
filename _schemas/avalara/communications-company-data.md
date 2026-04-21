---
description: CompanyData schema from Avalara API
layout: schema
name: CompanyData
properties_list:
- description: Business class (0=ILEC, 1=CLEC, etc.)
  name: bscl
  type: integer
- description: Service class (0=Primary Local, 1=Primary Long Distance)
  name: svcl
  type: integer
- description: Facilities-based indicator
  name: fclt
  type: boolean
- description: Franchise indicator
  name: frch
  type: boolean
- description: Regulated indicator
  name: reg
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-company-data-schema.json
slug: communications-company-data
tags:
- Taxes
title: CompanyData
---
