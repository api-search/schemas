---
description: List of the statistics such as the average age, tenure, compensation of leadership, the number of executives, and the gender diversity of leadership for the requested identifier.
layout: schema
name: companyStats
properties_list:
- description: Average compensation for the executives
  name: averageMgmtCompensation
  type: number
- description: Avergae tenure of the people
  name: averageTenure
  type: number
- description: Median tenure
  name: medianTenure
  type: number
- description: Average of the executives on the management and board
  name: averageAge
  type: number
- description: Maximum age of the people on Management & Board
  name: maxAge
  type: number
- description: Minimum age of the person on board
  name: minimumAge
  type: number
- description: Median age of the people on board
  name: medianAge
  type: number
- description: Independent directors on the board
  name: boardIndependentDirectors
  type: number
- description: Number of female members on the board
  name: femaleBoardMembers
  type: number
- description: Percentage of female members on the board
  name: femaleBoardMembersPercent
  type: number
- description: Number of people on board.
  name: numberOfMembers
  type: number
- description: On Other Boards All
  name: onOtherBoardsAll
  type: number
- description: On Other Boards Corporate
  name: onOtherBoardsCorporate
  type: number
- description: Management and Board type, where MB = Management & Board, MGMT = Management, and BRD = Board. This is a pass-through value from the input used in the `mbType` query parameter.
  name: mbType
  type: string
- description: Original identifier used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-people-company-stats-schema.json
slug: factset-people-company-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"companyStats\",\n  \"type\": \"object\",\n  \"description\": \"List of the statistics such as the average age, tenure, compensation of leadership, the number of executives, and the gender diversity of leadership for the requested identifier.\",\n  \"properties\": {\n    \"averageMgmtCompensation\": {\n      \"type\": \"number\",\n      \"description\": \"Average compensation for the executives\"\n    },\n    \"averageTenure\": {\n      \"type\": \"number\",\n      \"description\": \"Avergae tenure of the people\"\n    },\n    \"medianTenure\": {\n      \"type\": \"number\",\n      \"description\": \"Median tenure\"\n    },\n    \"averageAge\": {\n      \"type\": \"number\",\n      \"description\": \"Average of the executives on the management and board\"\n    },\n    \"maxAge\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum age of the people on Management & Board\"\n    },\n\
  \    \"minimumAge\": {\n      \"type\": \"number\",\n      \"description\": \"Minimum age of the person on board\"\n    },\n    \"medianAge\": {\n      \"type\": \"number\",\n      \"description\": \"Median age of the people on board\"\n    },\n    \"boardIndependentDirectors\": {\n      \"type\": \"number\",\n      \"description\": \"Independent directors on the board\"\n    },\n    \"femaleBoardMembers\": {\n      \"type\": \"number\",\n      \"description\": \"Number of female members on the board\"\n    },\n    \"femaleBoardMembersPercent\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage of female members on the board\"\n    },\n    \"numberOfMembers\": {\n      \"type\": \"number\",\n      \"description\": \"Number of people on board.\"\n    },\n    \"onOtherBoardsAll\": {\n      \"type\": \"number\",\n      \"description\": \"On Other Boards All\"\n    },\n    \"onOtherBoardsCorporate\": {\n      \"type\": \"number\",\n      \"description\": \"On Other Boards\
  \ Corporate\"\n    },\n    \"mbType\": {\n      \"type\": \"string\",\n      \"description\": \"Management and Board type, where MB = Management & Board, MGMT = Management, and BRD = Board. This is a pass-through value from the input used in the `mbType` query parameter.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Original identifier used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-people-company-stats-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: companyStats
---
