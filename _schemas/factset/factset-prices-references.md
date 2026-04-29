---
description: ''
layout: schema
name: references
properties_list:
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: The name of the security.
  name: name
  type: string
- description: 'Security Type Description. For more details, visit [Online Assistant Page #10149](https://oa.apps.factset.com/pages/10149).'
  name: secType
  type: string
- description: 'General Security Type Code. For more details regarding what the code represents, visit [Online Assistant Page #10149](https://oa.apps.factset.com/pages/10149).'
  name: secTypeCode
  type: string
- description: 'Detailed Security Type Code. For more details regarding what the code represents, visit [Online Assistant Page #10149](https://oa.apps.factset.com/pages/10149).'
  name: secTypeCodeDet
  type: string
- description: 'Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).'
  name: currency
  type: string
- description: 'Country Name. Returns the country where the security is *traded* from the North American Pricing database. Therefore, for securities covered by the North American Pricing database, will return either '
  name: country
  type: string
- description: 'Primary Exchange Name. For more details, visit [Online Assistant Page #16610](https://oa.apps.factset.com/pages/16610).'
  name: primaryExchange
  type: string
- description: Returns the location of the exchange where the company's stock is traded.
  name: exchangeCountry
  type: string
- description: 'The Local Index ID for the company''s home country benchmark. For more details, visit [Online Assistant Page #10698](https://oa.apps.factset.com/pages/10698).'
  name: localIndex
  type: string
- description: 'The Next Trading Holiday. For more details regarding Global Trading Holiday Schedules, visit [Online Assistant Page #10397](https://oa.apps.factset.com/pages/10397).'
  name: nextTradingHolidayDate
  type: string
- description: The Security's Date of First Trade. It will return the first date that the FactSet Pricing database began to cover the security and it may not coincide with the actual IPO date. Pricing information fo
  name: firstDate
  type: string
- description: Date of Last Trade. It will return the last date that the FactSet Pricing database as a record for this security listing.
  name: lastDate
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-prices-references-schema.json
slug: factset-prices-references
source_filename: factset-prices-references-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"references\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the security.\"\n    },\n    \"secType\": {\n      \"type\": \"string\",\n      \"description\": \"Security Type Description. For more details, visit [Online Assistant Page #10149](https://oa.apps.factset.com/pages/10149).\"\
  \n    },\n    \"secTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"General Security Type Code. For more details regarding what the code represents, visit [Online Assistant Page #10149](https://oa.apps.factset.com/pages/10149).\"\n    },\n    \"secTypeCodeDet\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed Security Type Code. For more details regarding what the code represents, visit [Online Assistant Page #10149](https://oa.apps.factset.com/pages/10149).\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency ISO code. For more details, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country Name. Returns the country where the security is *traded* from the North American Pricing database. Therefore, for securities covered by the North American Pricing database, will return either UNITED STATES.\
  \ or CANADA. For securities covered by the Global Pricing database, the item returns the country where the company is *incorporated*.\"\n    },\n    \"primaryExchange\": {\n      \"type\": \"string\",\n      \"description\": \"Primary Exchange Name. For more details, visit [Online Assistant Page #16610](https://oa.apps.factset.com/pages/16610).\"\n    },\n    \"exchangeCountry\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the location of the exchange where the company's stock is traded.\"\n    },\n    \"localIndex\": {\n      \"type\": \"string\",\n      \"description\": \"The Local Index ID for the company's home country benchmark. For more details, visit [Online Assistant Page #10698](https://oa.apps.factset.com/pages/10698).\"\n    },\n    \"nextTradingHolidayDate\": {\n      \"type\": \"string\",\n      \"description\": \"The Next Trading Holiday. For more details regarding Global Trading Holiday Schedules, visit [Online Assistant Page #10397](https://oa.apps.factset.com/pages/10397).\"\
  \n    },\n    \"firstDate\": {\n      \"type\": \"string\",\n      \"description\": \"The Security's Date of First Trade. It will return the first date that the FactSet Pricing database began to cover the security and it may not coincide with the actual IPO date. Pricing information for this security will not be available before the date returned. For more details.\"\n    },\n    \"lastDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of Last Trade.  It will return the last date that the FactSet Pricing database as a record for this security listing.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-prices-references-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: references
---
