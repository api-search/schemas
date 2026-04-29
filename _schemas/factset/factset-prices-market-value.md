---
description: ''
layout: schema
name: marketValue
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: Ending date for the period expressed in YYYY-MM-DD format.
  name: date
  type: string
- description: 'Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).'
  name: currency
  type: string
- description: Aggregate market value across all share classes and includes non-traded shares which are added to the calculation basis by the proportion of their nominal or par value. Values are in base units. To va
  name: entityMarketValue
  type: number
- description: 'Aggregate across all share classes and excludes non-traded shares. Values are in base units. For more details visit [Online Assistant Page #16867](https://my.apps.factset.com/oa/pages/16867).'
  name: entityMarketValueExNonTraded
  type: number
- description: Returns the security level market value calculated as the share price multiplied by the number of shares at the security level. **Note:** History is available back to Oct-1999 for North American secur
  name: securityMarketValue
  type: number
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-market-value-schema.json
slug: factset-prices-market-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"marketValue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Ending date for the period expressed in YYYY-MM-DD format.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\
  \n    },\n    \"entityMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Aggregate market value across all share classes and includes non-traded shares which are added to the calculation basis by the proportion of their nominal or par value. Values are in base units. To value non-traded shares, the price of the parent equity provides the most appropriate approximation of what the non-traded shares would be worth in the open market. For unique companies with an ADR as the parent equity, since it is the only traded security associated with that company, when calculating company-level market value, the price of the ADR is used, but is scaled by the ADR ratio since there's not always a one-to-one relationship between ADR shares and the non-traded shares which they represent. For more details visit [Online Assistant Page #16867](https://my.apps.factset.com/oa/pages/16867). \"\n    },\n    \"entityMarketValueExNonTraded\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Aggregate across all share classes and excludes non-traded shares. Values are in base units. For more details visit [Online Assistant Page #16867](https://my.apps.factset.com/oa/pages/16867).\"\n    },\n    \"securityMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the security level market value calculated as the share price multiplied by the number of shares at the security level. **Note:** History is available back to Oct-1999 for North American securities, and 1-Jan-2001 for non-North American securities.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-market-value-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: marketValue
---
