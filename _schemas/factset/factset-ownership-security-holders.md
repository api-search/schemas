---
description: Security Holders response object
layout: schema
name: securityHolders
properties_list:
- description: FactSet Ownership Holders ID that corresponds to the requested security holder.
  name: holderId
  type: string
- description: FactSet Security Identifier of security requested. This does not represent the FactSet permanent identifier for the holder, but rather the requested id. Six alpha-numeric characters, excluding vowels,
  name: fsymId
  type: string
- description: FactSet Entity ID that corresponds to the specified holder ID.
  name: holderEntityId
  type: string
- description: Name of the holder for the requested security identifier.
  name: holderName
  type: string
- description: 'Date of the reported holding in YYYY-MM-DD format. For more details regarding date resolution, visit [Online Assistant Page #11262](https://oa.apps.factset.com/pages/11262).'
  name: date
  type: string
- description: 'Currency code. The service will default to the local currency if the currency is not requested. For a list of currency ISO codes, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/'
  name: currency
  type: string
- description: 'FactSet Ownership Institution, Mutual Fund, and Insider/Stakeholder investor types. To learn more about the different investor types, visit [Online Assistant Page #11656](https://my.apps.factset.com/o'
  name: investorType
  type: string
- description: Holder Type name of the respective holder object. The name will align to the holderType requested.
  name: holderType
  type: string
- description: Adjusted number of shares held. All positions and prices are adjusted for splits and name changes, but they are not adjusted for spinoffs or mergers. If a given company announces a split today, FactSe
  name: adjHolding
  type: number
- description: 'Adjusted market values of shares held. Market Value. All positions and prices are adjusted for splits and name changes, but they are not adjusted for spinoffs or mergers. If a given company announces '
  name: adjMarketValue
  type: number
- description: '"Closing weight of the security for the holders of the requested security (percent). To learn more about how ownership weight is calculated please visit [Online Assistant Page #11247](https://my.apps.'
  name: weightClose
  type: number
- description: 'The percent of the outstanding common shares held by a particular filing institution. To learn more, visit [Online Assistant Page #11041](https://my.apps.factset.com/oa/pages/11041).'
  name: percentOutstanding
  type: number
- description: Either the 13F Form or ND-30D report filed where the security holdings data was sourced from. To learn more about source, please visit https://my.apps.factset.com/oa/pages/11260
  name: source
  type: string
- description: Security Identifier that was used in the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-ownership-security-holders-schema.json
slug: factset-ownership-security-holders
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"securityHolders\",\n  \"type\": \"object\",\n  \"description\": \"Security Holders response object\",\n  \"properties\": {\n    \"holderId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Ownership Holders ID that corresponds to the requested security holder.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier of security requested. This does not represent the FactSet permanent identifier for the holder, but rather the requested id. Six alpha-numeric characters, excluding vowels, with an -S suffix (XXXXXX-S). All equity and fixed income securities that exist on FactSet are allocated a security-level permanent identifier.\"\n    },\n    \"holderEntityId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity ID that corresponds to the specified holder ID.\"\n    },\n    \"holderName\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Name of the holder for the requested security identifier.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the reported holding in YYYY-MM-DD format. For more details regarding date resolution, visit [Online Assistant Page #11262](https://oa.apps.factset.com/pages/11262).\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code. The service will default to the local currency if the currency is not requested. For a list of currency ISO codes, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n    \"investorType\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Ownership Institution, Mutual Fund, and Insider/Stakeholder investor types. To learn more about the different investor types, visit [Online Assistant Page #11656](https://my.apps.factset.com/oa/pages/11656).\"\n    },\n    \"holderType\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Holder Type name of the respective holder object. The name will align to the holderType requested. \"\n    },\n    \"adjHolding\": {\n      \"type\": \"number\",\n      \"description\": \"Adjusted number of shares held. All positions and prices are adjusted for splits and name changes, but they are not adjusted for spinoffs or mergers. If a given company announces a split today, FactSet's Ownership data will reflect that split either tomorrow or the day after, depending upon the time in which the FactSet Symbology team makes record of the change. For more details, visit [Online Assistant Page #11262](https://oa.apps.factset.com/pages/11262).\"\n    },\n    \"adjMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Adjusted market values of shares held. Market Value. All positions and prices are adjusted for splits and name changes, but they are not adjusted for spinoffs or mergers. If a given company announces a split today,\
  \ FactSet's Ownership data will reflect that split either tomorrow or the day after, depending upon the time in which the FactSet Symbology team makes record of the change. For more details, visit [Online Assistant Page #11262](https://oa.apps.factset.com/pages/11262).\"\n    },\n    \"weightClose\": {\n      \"type\": \"number\",\n      \"description\": \"\\\"Closing weight of the security for the holders of the requested security (percent). To learn more about how ownership weight is calculated please visit [Online Assistant Page #11247](https://my.apps.factset.com/oa/pages/11247).\\\"\\n\"\n    },\n    \"percentOutstanding\": {\n      \"type\": \"number\",\n      \"description\": \"The percent of the outstanding common shares held by a particular filing institution. To learn more, visit [Online Assistant Page #11041](https://my.apps.factset.com/oa/pages/11041).\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Either the 13F Form or ND-30D report filed\
  \ where the security holdings data was sourced from. To learn more about source, please visit https://my.apps.factset.com/oa/pages/11260\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Security Identifier that was used in the request.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-ownership-security-holders-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: securityHolders
---
