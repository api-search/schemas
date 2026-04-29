---
description: ''
layout: schema
name: detailRatings
properties_list:
- description: ''
  name: fsymId
  type: string
- description: 'Date of estimate expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)'
  name: estimateDate
  type: string
- description: The FactSet Entity Identifier for the analyst making the estimate.
  name: analystId
  type: string
- description: The name of the analyst making the estimate.
  name: analystName
  type: string
- description: The FactSet Entity Identifier for the broker making the estimate.
  name: brokerId
  type: string
- description: The name of the broker making the estimate.
  name: brokerName
  type: string
- description: 'A textual representation of the analysts rating. Broker recommendations are divided into five main broad categories- **Buy, Overweight, Hold, Underweight, and Sell**.<p>Additional recommendations may '
  name: ratingsNoteText
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: Date and time when the data is available at the source.
  name: inputDateTime
  type: string
- description: The date at which a broker provided an estimate that is a revision.
  name: lastModifiedDate
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-estimates-detail-ratings-schema.json
slug: factset-estimates-detail-ratings
source_filename: factset-estimates-detail-ratings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"detailRatings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\"\n    },\n    \"estimateDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of estimate expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)\"\n    },\n    \"analystId\": {\n      \"type\": \"string\",\n      \"description\": \"The FactSet Entity Identifier for the analyst making the estimate.\"\n    },\n    \"analystName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the analyst making the estimate.\"\n    },\n    \"brokerId\": {\n      \"type\": \"string\",\n      \"description\": \"The FactSet Entity Identifier for the broker making the estimate.\"\n    },\n    \"brokerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the broker making the\
  \ estimate.\"\n    },\n    \"ratingsNoteText\": {\n      \"type\": \"string\",\n      \"description\": \"A textual representation of the analysts rating. Broker recommendations are divided into five main broad categories- **Buy, Overweight, Hold, Underweight, and Sell**.<p>Additional recommendations may be displayed for the below reasons - \\n* Without- A rating \\\"Without\\\" is displayed when a broker provides estimates but does not provide a rating.\\n* Dropping- When a broker stops covering an equity, the recommendation will show \\\"Dropping.\\\"\\n* Not Available- A broker may be \\\"Not Available\\\" due to outstanding circumstances with that particular security. Ratings are not displayed until a new rating is provided.\\n* Most/Least- \\\"Most\\\" or \\\"Least\\\" favorable rating is displayed for top or bottom rating available for a particular security.\\n\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\
  \n    },\n    \"inputDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the data is available at the source.\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date at which a broker provided an estimate that is a revision.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-estimates-detail-ratings-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: detailRatings
---
