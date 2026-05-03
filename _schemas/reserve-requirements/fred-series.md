---
description: JSON Schema for a FRED (Federal Reserve Economic Data) time series object. Key reserve-related series include RESBALNS (reserve balances with Federal Reserve Banks), BOGMBASE (monetary base), and WRESBAL (reserve balances).
layout: schema
name: FRED Economic Data Series
properties_list:
- description: Series ID (e.g., RESBALNS, BOGMBASE, WRESBAL).
  name: id
  type: string
- description: Realtime start date.
  name: realtime_start
  type: string
- description: Realtime end date.
  name: realtime_end
  type: string
- description: Series title.
  name: title
  type: string
- description: Start date of available observations.
  name: observation_start
  type: string
- description: End date of available observations.
  name: observation_end
  type: string
- description: Data frequency.
  name: frequency
  type: string
- description: Short frequency code.
  name: frequency_short
  type: string
- description: Data units.
  name: units
  type: string
- description: Short units description.
  name: units_short
  type: string
- description: Seasonal adjustment status.
  name: seasonal_adjustment
  type: string
- description: Short seasonal adjustment code.
  name: seasonal_adjustment_short
  type: string
- description: Last update timestamp.
  name: last_updated
  type: string
- description: Popularity score (0-100).
  name: popularity
  type: integer
- description: Series notes and descriptions.
  name: notes
  type: string
provider_name: Reserve Requirements
provider_slug: reserve-requirements
schema_file: json-schema/fred-series-schema.json
slug: fred-series
source_filename: fred-series-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/reserve-requirements/json-schema/fred-series-schema.json\",\n  \"title\": \"FRED Economic Data Series\",\n  \"description\": \"JSON Schema for a FRED (Federal Reserve Economic Data) time series object. Key reserve-related series include RESBALNS (reserve balances with Federal Reserve Banks), BOGMBASE (monetary base), and WRESBAL (reserve balances).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Series ID (e.g., RESBALNS, BOGMBASE, WRESBAL).\",\n      \"example\": \"RESBALNS\"\n    },\n    \"realtime_start\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Realtime start date.\"\n    },\n    \"realtime_end\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Realtime end date.\"\n    },\n    \"title\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Series title.\",\n      \"example\": \"Reserve Balances with Federal Reserve Banks\"\n    },\n    \"observation_start\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of available observations.\"\n    },\n    \"observation_end\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date of available observations.\"\n    },\n    \"frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Data frequency.\",\n      \"example\": \"Weekly, Ending Wednesday\"\n    },\n    \"frequency_short\": {\n      \"type\": \"string\",\n      \"description\": \"Short frequency code.\",\n      \"example\": \"W\"\n    },\n    \"units\": {\n      \"type\": \"string\",\n      \"description\": \"Data units.\",\n      \"example\": \"Millions of Dollars\"\n    },\n    \"units_short\": {\n      \"type\": \"string\",\n      \"description\": \"Short units description.\",\n   \
  \   \"example\": \"Mil. of $\"\n    },\n    \"seasonal_adjustment\": {\n      \"type\": \"string\",\n      \"description\": \"Seasonal adjustment status.\",\n      \"example\": \"Not Seasonally Adjusted\"\n    },\n    \"seasonal_adjustment_short\": {\n      \"type\": \"string\",\n      \"description\": \"Short seasonal adjustment code.\",\n      \"example\": \"NSA\"\n    },\n    \"last_updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update timestamp.\"\n    },\n    \"popularity\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Popularity score (0-100).\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Series notes and descriptions.\"\n    }\n  },\n  \"required\": [\"id\", \"title\", \"frequency\", \"units\", \"observation_start\", \"observation_end\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reserve-requirements/refs/heads/main/json-schema/fred-series-schema.json
tags:
- Reserve Requirements
- Federal Reserve
- Banking Regulation
- Monetary Policy
- Regulation D
- Finance
title: FRED Economic Data Series
---
