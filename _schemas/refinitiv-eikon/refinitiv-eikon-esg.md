---
description: Schema for ESG (Environmental, Social, and Governance) scores from the Refinitiv Eikon Data Platform.
layout: schema
name: Refinitiv Eikon ESG Score
properties_list:
- description: Instrument identifier (RIC or PermID).
  name: instrumentId
  type: string
- description: Overall ESG combined score (0-100).
  name: esgScore
  type: number
- description: Combined ESG score including controversies impact.
  name: esgCombinedScore
  type: number
- description: Environmental pillar score covering resource use, emissions, and innovation.
  name: environmentPillarScore
  type: number
- description: Social pillar score covering workforce, human rights, community, and product responsibility.
  name: socialPillarScore
  type: number
- description: Corporate governance pillar score covering management, shareholders, and CSR strategy.
  name: governancePillarScore
  type: number
- description: Controversies score reflecting ESG incidents and controversies.
  name: controversiesScore
  type: number
- description: Reporting period for the ESG scores.
  name: period
  type: string
- description: Detailed ESG measure fields keyed by field name.
  name: measures
  type: object
provider_name: Refinitiv Eikon
provider_slug: refinitiv-eikon
schema_file: json-schema/refinitiv-eikon-esg-schema.json
slug: refinitiv-eikon-esg
source_filename: refinitiv-eikon-esg-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/refinitiv-eikon/json-schema/refinitiv-eikon-esg-schema.json\",\n  \"title\": \"Refinitiv Eikon ESG Score\",\n  \"description\": \"Schema for ESG (Environmental, Social, and Governance) scores from the Refinitiv Eikon Data Platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instrumentId\": {\n      \"type\": \"string\",\n      \"description\": \"Instrument identifier (RIC or PermID).\"\n    },\n    \"esgScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Overall ESG combined score (0-100).\"\n    },\n    \"esgCombinedScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Combined ESG score including controversies impact.\"\n    },\n    \"environmentPillarScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\"\
  : 100,\n      \"description\": \"Environmental pillar score covering resource use, emissions, and innovation.\"\n    },\n    \"socialPillarScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Social pillar score covering workforce, human rights, community, and product responsibility.\"\n    },\n    \"governancePillarScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Corporate governance pillar score covering management, shareholders, and CSR strategy.\"\n    },\n    \"controversiesScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Controversies score reflecting ESG incidents and controversies.\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"Reporting period for the ESG scores.\",\n      \"examples\": [\"FY2023\", \"FY2022\"]\n    },\n    \"measures\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Detailed ESG measure fields keyed by field name.\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          {\"type\": \"number\"},\n          {\"type\": \"string\"},\n          {\"type\": \"boolean\"},\n          {\"type\": \"null\"}\n        ]\n      }\n    }\n  },\n  \"required\": [\"instrumentId\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/json-schema/refinitiv-eikon-esg-schema.json
tags:
- Analytics
- Financial Data
- Financial News
- Market Data
- Real-Time Data
- Trading
title: Refinitiv Eikon ESG Score
---
