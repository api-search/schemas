---
description: ''
layout: schema
name: EarningsReport
properties_list:
- description: Fiscal year
  name: year
  type: integer
- description: Quarter (null for annual)
  name: quarter
  type: integer
- description: Total revenue in USD
  name: revenue
  type: integer
- description: Adjusted EBITDA in USD
  name: ebitda
  type: integer
- description: Net income in USD
  name: netIncome
  type: integer
- description: Diluted earnings per share in USD
  name: earningsPerShare
  type: number
provider_name: Arch Coal
provider_slug: arch-coal
schema_file: json-schema/arch-coal-investor-relations-api-earnings-report-schema.json
slug: arch-coal-investor-relations-api-earnings-report
tags:
- Mining
- Coal
- Metallurgical Coal
- Thermal Coal
- Energy
- Fortune 500
title: EarningsReport
---
