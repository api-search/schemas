---
description: ''
layout: schema
name: consensusRatings
properties_list:
- description: ''
  name: fsymId
  type: string
- description: 'Date of estimate expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)'
  name: estimateDate
  type: string
- description: The number of Buy ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.
  name: buyCount
  type: integer
- description: The number of Overweight ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.
  name: overweightCount
  type: integer
- description: The number of Hold ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.
  name: holdCount
  type: integer
- description: The number of Underweight ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.
  name: underweightCount
  type: integer
- description: The number of Sell ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.
  name: sellCount
  type: integer
- description: The total number of ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.
  name: ratingsNestTotal
  type: integer
- description: The mean average of ratings for the fiscal dates indicated, where each underlying rating is given a numerical score and then aggregated to a mean consensus - __*Individual Ratings Scores*__ |Value|Rat
  name: ratingsNote
  type: number
- description: The mean textual rating for the fiscal dates indicated. The text rating is assigned by falling within the below defined ranges - __*Textual Ranges for Average*__ |Value|Rating Description| ||| |< 1.25
  name: ratingsNoteText
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-estimates-consensus-ratings-schema.json
slug: factset-estimates-consensus-ratings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"consensusRatings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\"\n    },\n    \"estimateDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of estimate expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)\"\n    },\n    \"buyCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of Buy ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.\"\n    },\n    \"overweightCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of Overweight ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.\"\n    },\n    \"holdCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number\
  \ of Hold ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.\"\n    },\n    \"underweightCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of Underweight ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.\"\n    },\n    \"sellCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of Sell ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.\"\n    },\n    \"ratingsNestTotal\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of ratings taken into account in the calculation of a consensus. This information is shown only for a 100-day consensus.\"\n    },\n    \"ratingsNote\": {\n      \"type\": \"number\",\n      \"description\": \"The mean average of ratings for the fiscal dates indicated, where each underlying rating\
  \ is given a numerical score and then aggregated to a mean consensus -\\n__*Individual Ratings Scores*__\\n|Value|Rating Description|\\n|||\\n|1|Buy|\\n|1.5|Overweight|\\n|2|Hold|\\n|2.5|Underweight|\\n|3|Sell|\\n\"\n    },\n    \"ratingsNoteText\": {\n      \"type\": \"string\",\n      \"description\": \"The mean textual rating for the fiscal dates indicated. The text rating is assigned by falling within the below defined ranges - \\n__*Textual Ranges for Average*__\\n|Value|Rating Description|\\n|||\\n|< 1.25|Buy|\\n|< 1.75|Overweight|\\n|< 2.25|Hold|\\n|< 2.75|Underweight|\\n|<= 3|Sell|\\n\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-estimates-consensus-ratings-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: consensusRatings
---
