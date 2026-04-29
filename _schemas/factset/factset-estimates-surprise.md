---
description: ''
layout: schema
name: surprise
properties_list:
- description: ''
  name: fsymId
  type: string
- description: Date for data expressed in YYYY-MM-DD format.
  name: date
  type: string
- description: 'Currency code for adjusting the data. Use ''ESTIMATE'' as input value for the values in Estimate Currency. For a list of currency ISO codes, visit [Online Assistant Page #1470](https://oa.apps.factset.c'
  name: currency
  type: string
- description: Estimate currency of the requested Security
  name: estimateCurrency
  type: string
- description: 'Company''s Financial statement ''metric'' that is estimated. Use the factset-estimates/v#/metrics endpoint for a complete list. For more details, visit [Online Assistant Page #15034](https://oa.apps.fact'
  name: metric
  type: string
- description: 'Method of calculation for the consensus ''statistic''. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114).'
  name: statistic
  type: string
- description: Company's 'periodicity' for the estimate record, reflecting Annual, Quarterly, or Semi-Annual report periods. Next-twelve-months (NTMA) and Last-twelve-months (LTMA) also supported.
  name: periodicity
  type: string
- description: Company's 'fiscal end date' for the estimate record expressed in YYYY-MM-DD format
  name: fiscalEndDate
  type: string
- description: Company's 'fiscal year' for the estimate record
  name: fiscalYear
  type: integer
- description: Company's 'fiscal period' for the estimate record. 'Periodicity' defines context for period.
  name: fiscalPeriod
  type: integer
- description: 'Date of the reported event expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16601](https://oa.apps.factset.com/pages/16601).'
  name: surpriseDate
  type: string
- description: 'Amount of difference between last consensus and actual. For more details, visit [Online Assistant Page #16145](https://oa.apps.factset.com/pages/16145).'
  name: surpriseAmount
  type: number
- description: 'Percent difference between last consensus and actual. For more details, visit [Online Assistant Page #16145](https://oa.apps.factset.com/pages/16145).'
  name: surprisePercent
  type: number
- description: 'Last consensus before event. For more details, visit [Online Assistant Page #16145](https://oa.apps.factset.com/pages/16145).'
  name: surpriseBefore
  type: number
- description: 'Actual value after event. For more details, visit [Online Assistant Page #16145](https://oa.apps.factset.com/pages/16145).'
  name: surpriseAfter
  type: number
- description: 'Description of event. For more details, visit [Online Assistant Page #16601](https://oa.apps.factset.com/pages/16601).'
  name: eventDescription
  type: string
- description: 'Flag for event. Code of Event Flag, where 0 = results and 1 = profit warning. For more details, visit [Online Assistant Page #16601](https://oa.apps.factset.com/pages/16601).'
  name: eventFlag
  type: integer
- description: ''
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-estimates-surprise-schema.json
slug: factset-estimates-surprise
source_filename: factset-estimates-surprise-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"surprise\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date for data expressed in YYYY-MM-DD format.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code for adjusting the data. Use 'ESTIMATE' as input value for the values in Estimate Currency. For a list of currency ISO codes, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"estimateCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Estimate currency of the requested Security\"\n    },\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"Company's Financial statement 'metric' that is estimated. Use the factset-estimates/v#/metrics endpoint for a complete list. For more details, visit\
  \ [Online Assistant Page #15034](https://oa.apps.factset.com/pages/15034).\"\n    },\n    \"statistic\": {\n      \"type\": \"string\",\n      \"description\": \"Method of calculation for the consensus 'statistic'. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114).\"\n    },\n    \"periodicity\": {\n      \"type\": \"string\",\n      \"description\": \"Company's 'periodicity' for the estimate record, reflecting Annual, Quarterly, or Semi-Annual report periods. Next-twelve-months (NTMA) and Last-twelve-months (LTMA) also supported.\"\n    },\n    \"fiscalEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"Company's 'fiscal end date' for the estimate record expressed in YYYY-MM-DD format\"\n    },\n    \"fiscalYear\": {\n      \"type\": \"integer\",\n      \"description\": \"Company's 'fiscal year' for the estimate record\"\n    },\n    \"fiscalPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Company's 'fiscal\
  \ period' for the estimate record.  'Periodicity' defines context for period.\"\n    },\n    \"surpriseDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the reported event expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16601](https://oa.apps.factset.com/pages/16601).\"\n    },\n    \"surpriseAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount of difference between last consensus and actual. For more details, visit [Online Assistant Page #16145](https://oa.apps.factset.com/pages/16145).\"\n    },\n    \"surprisePercent\": {\n      \"type\": \"number\",\n      \"description\": \"Percent difference between last consensus and actual. For more details, visit [Online Assistant Page #16145](https://oa.apps.factset.com/pages/16145).\"\n    },\n    \"surpriseBefore\": {\n      \"type\": \"number\",\n      \"description\": \"Last consensus before event. For more details, visit [Online Assistant Page #16145](https://oa.apps.factset.com/pages/16145).\"\
  \n    },\n    \"surpriseAfter\": {\n      \"type\": \"number\",\n      \"description\": \"Actual value after event. For more details, visit [Online Assistant Page #16145](https://oa.apps.factset.com/pages/16145).\"\n    },\n    \"eventDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Description of event. For more details, visit [Online Assistant Page #16601](https://oa.apps.factset.com/pages/16601).\"\n    },\n    \"eventFlag\": {\n      \"type\": \"integer\",\n      \"description\": \"Flag for event. Code of Event Flag, where 0 = results and 1 = profit warning. For more details, visit [Online Assistant Page #16601](https://oa.apps.factset.com/pages/16601).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-estimates-surprise-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: surprise
---
