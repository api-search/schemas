---
description: Environmental, Social, and Governance score data for a company as provided by the Refinitiv Data Platform ESG API, including overall scores, pillar scores, and category-level measures.
layout: schema
name: Refinitiv ESG Score
properties_list:
- description: The instrument identifier (RIC or PermID) for the scored company.
  name: instrumentId
  type: string
- description: The company name associated with the ESG score.
  name: companyName
  type:
  - string
  - 'null'
- description: The fiscal period end date for the ESG assessment.
  name: periodEndDate
  type: string
- description: Overall ESG score combining all three pillars, ranging from 0 to 100.
  name: esgScore
  type:
  - number
  - 'null'
- description: Combined ESG score factoring in controversies, ranging from 0 to 100.
  name: esgCombinedScore
  type:
  - number
  - 'null'
- description: Environmental pillar score measuring resource use, emissions, and innovation, ranging from 0 to 100.
  name: environmentPillarScore
  type:
  - number
  - 'null'
- description: Social pillar score measuring workforce, human rights, community, and product responsibility, ranging from 0 to 100.
  name: socialPillarScore
  type:
  - number
  - 'null'
- description: Governance pillar score measuring management, shareholders, and CSR strategy, ranging from 0 to 100.
  name: governancePillarScore
  type:
  - number
  - 'null'
- description: ESG grade on a letter scale from D- to A+.
  name: esgGrade
  type:
  - string
  - 'null'
- description: Controversies score reflecting ESG-related negative news events, ranging from 0 to 100.
  name: controversiesScore
  type:
  - number
  - 'null'
- description: Total CO2 equivalent emissions in tonnes.
  name: co2Emissions
  type:
  - number
  - 'null'
- description: Direct CO2 emissions (Scope 1) in tonnes.
  name: co2EmissionsScope1
  type:
  - number
  - 'null'
- description: Indirect CO2 emissions from purchased energy (Scope 2) in tonnes.
  name: co2EmissionsScope2
  type:
  - number
  - 'null'
- description: The TRBC industry classification of the company.
  name: industry
  type:
  - string
  - 'null'
- description: The country of domicile of the company.
  name: country
  type:
  - string
  - 'null'
provider_name: Refinitiv
provider_slug: refinitiv
schema_file: json-schema/refinitiv-esg-score-schema.json
slug: refinitiv-esg-score
source_filename: refinitiv-esg-score-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.refinitiv.com/schemas/refinitiv/esg-score.json\",\n  \"title\": \"Refinitiv ESG Score\",\n  \"description\": \"Environmental, Social, and Governance score data for a company as provided by the Refinitiv Data Platform ESG API, including overall scores, pillar scores, and category-level measures.\",\n  \"type\": \"object\",\n  \"required\": [\"instrumentId\", \"periodEndDate\"],\n  \"properties\": {\n    \"instrumentId\": {\n      \"type\": \"string\",\n      \"description\": \"The instrument identifier (RIC or PermID) for the scored company.\"\n    },\n    \"companyName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The company name associated with the ESG score.\"\n    },\n    \"periodEndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The fiscal period end date for the ESG assessment.\"\n    },\n    \"esgScore\"\
  : {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Overall ESG score combining all three pillars, ranging from 0 to 100.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"esgCombinedScore\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Combined ESG score factoring in controversies, ranging from 0 to 100.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"environmentPillarScore\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Environmental pillar score measuring resource use, emissions, and innovation, ranging from 0 to 100.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"socialPillarScore\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Social pillar score measuring workforce, human rights, community, and product responsibility, ranging from 0 to 100.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"governancePillarScore\": {\n      \"\
  type\": [\"number\", \"null\"],\n      \"description\": \"Governance pillar score measuring management, shareholders, and CSR strategy, ranging from 0 to 100.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"esgGrade\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ESG grade on a letter scale from D- to A+.\",\n      \"enum\": [\"A+\", \"A\", \"A-\", \"B+\", \"B\", \"B-\", \"C+\", \"C\", \"C-\", \"D+\", \"D\", \"D-\", null]\n    },\n    \"controversiesScore\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Controversies score reflecting ESG-related negative news events, ranging from 0 to 100.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"co2Emissions\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Total CO2 equivalent emissions in tonnes.\",\n      \"minimum\": 0\n    },\n    \"co2EmissionsScope1\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Direct CO2 emissions\
  \ (Scope 1) in tonnes.\",\n      \"minimum\": 0\n    },\n    \"co2EmissionsScope2\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Indirect CO2 emissions from purchased energy (Scope 2) in tonnes.\",\n      \"minimum\": 0\n    },\n    \"industry\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The TRBC industry classification of the company.\"\n    },\n    \"country\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The country of domicile of the company.\"\n    }\n  },\n  \"$defs\": {\n    \"CategoryScore\": {\n      \"type\": \"object\",\n      \"description\": \"An individual ESG category score within a pillar.\",\n      \"properties\": {\n        \"categoryName\": {\n          \"type\": \"string\",\n          \"description\": \"The category name such as Resource Use, Emissions, or Workforce.\"\n        },\n        \"score\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"The category score\
  \ ranging from 0 to 100.\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"pillar\": {\n          \"type\": \"string\",\n          \"description\": \"The parent pillar for this category.\",\n          \"enum\": [\"Environment\", \"Social\", \"Governance\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/json-schema/refinitiv-esg-score-schema.json
tags: []
title: Refinitiv ESG Score
---
