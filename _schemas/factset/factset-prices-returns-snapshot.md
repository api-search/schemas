---
description: ''
layout: schema
name: returnsSnapshot
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: Specific reference date for the period expressed in YYYY-MM-DD format.
  name: date
  type: string
- description: 'Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).'
  name: currency
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: Returns the price performance of the security for the previous one day from the given date.
  name: oneDay
  type: number
- description: Returns the price performance of the security for the past one month.
  name: oneMonth
  type: number
- description: Returns the price performance of the security for the past three months.
  name: threeMonth
  type: number
- description: Returns the price performance of the security for the past six months.
  name: sixMonth
  type: number
- description: Returns the price performance of the security for the past nine months.
  name: nineMonth
  type: number
- description: Returns the price performance of the security for the past one year.
  name: oneYear
  type: number
- description: Returns the price performance of the security from the previous calendar quarter end to the given date.
  name: quarterToDate
  type: number
- description: Returns the price performance of the security from the previous week (usually Friday) to the given date.
  name: weekToDate
  type: number
- description: Returns the price performance of the security from the previous month-end to the given date.
  name: monthToDate
  type: number
- description: Returns the price performance of the security from the previous calendar year-end to the given date.
  name: yearToDate
  type: number
- description: Returns the annualized compound total return for two years.
  name: twoYearAnnualized
  type: number
- description: Returns the annualized compound total return for three years.
  name: threeYearAnnualized
  type: number
- description: Returns the annualized compound total return for five years.
  name: fiveYearAnnualized
  type: number
- description: Returns the annualized compound total return for ten years.
  name: tenYearAnnualized
  type: number
- description: Returns the annualized compound total return for twenty years.
  name: twentyYearAnnualized
  type: number
- description: Returns the annualized compound total return for thirty years.
  name: thirtyYearAnnualized
  type: number
- description: Returns the annualized compound total return from the ipo date. The calculation uses the closing price as of the IPO date, and not the IPO price itself.
  name: ipoToDateAnnualized
  type: number
- description: 'Controls the dividend reinvestment for the returns calculation. Dividends will be reinvested on the date the dividends go ex (when the dividends belong to the seller rather than the buyer). Visit [OA '
  name: dividendAdjust
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-returns-snapshot-schema.json
slug: factset-prices-returns-snapshot
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"returnsSnapshot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Specific reference date for the period expressed in YYYY-MM-DD format.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code. For more details, visit [Online Assistant Page\
  \ #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    },\n    \"oneDay\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security for the previous one day from the given date.\"\n    },\n    \"oneMonth\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security for the past one month.\"\n    },\n    \"threeMonth\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security for the past three months.\"\n    },\n    \"sixMonth\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security for the past six months.\"\n    },\n    \"nineMonth\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security for the past nine months.\"\n    },\n\
  \    \"oneYear\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security for the past one year.\"\n    },\n    \"quarterToDate\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security from the previous calendar quarter end to the given date.\"\n    },\n    \"weekToDate\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security from the previous week (usually Friday) to the given date.\"\n    },\n    \"monthToDate\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security from the previous month-end to the given date.\"\n    },\n    \"yearToDate\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the price performance of the security from the previous calendar year-end to the given date.\"\n    },\n    \"twoYearAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"Returns\
  \ the annualized compound total return for two years.\"\n    },\n    \"threeYearAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the annualized compound total return for three years.\"\n    },\n    \"fiveYearAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the annualized compound total return for five years.\"\n    },\n    \"tenYearAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the annualized compound total return for ten years.\"\n    },\n    \"twentyYearAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the annualized compound total return for twenty years.\"\n    },\n    \"thirtyYearAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the annualized compound total return for thirty years.\"\n    },\n    \"ipoToDateAnnualized\": {\n      \"type\": \"number\",\n      \"description\": \"Returns the annualized compound total return from the ipo\
  \ date. The calculation uses the closing price as of the IPO date, and not the IPO price itself.\"\n    },\n    \"dividendAdjust\": {\n      \"type\": \"string\",\n      \"description\": \"Controls the dividend reinvestment for the returns calculation. Dividends will be reinvested on the date the dividends go ex (when the dividends belong to the seller rather than the buyer). Visit [OA 8748](https://my.apps.factset.com/oa/pages/8748) for calculation methodology.\\n  * **PRICE** = Price Change - Dividends Excluded.\\n  * **EXDATE** = Simple Return - Dividends Received on exdate but not reinvested. Dividends accumulated throughout the specified period are added to the price at the end of the period.\\n  * **EXDATE_C** = Compound Return - Dividends reinvested on exdate. Dividends accumulated throughout the specified period are used to buy more shares of stock in the company.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-returns-snapshot-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: returnsSnapshot
---
