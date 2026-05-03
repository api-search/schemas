---
description: A League of Legends match record from the Riot Games Match v5 API
layout: schema
name: Riot Games Match
properties_list:
- description: Match metadata
  name: metadata
  type: object
- description: Match information
  name: info
  type: object
provider_name: Riot Games
provider_slug: riot-games
schema_file: json-schema/riot-games-match-schema.json
slug: riot-games-match
source_filename: riot-games-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/riot-games/blob/main/json-schema/riot-games-match-schema.json\",\n  \"title\": \"Riot Games Match\",\n  \"description\": \"A League of Legends match record from the Riot Games Match v5 API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Match metadata\",\n      \"properties\": {\n        \"dataVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Match data version\"\n        },\n        \"matchId\": {\n          \"type\": \"string\",\n          \"description\": \"Match ID (e.g., NA1_4567890)\"\n        },\n        \"participants\": {\n          \"type\": \"array\",\n          \"description\": \"PUUIDs of all participants\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\"matchId\", \"participants\"]\n\
  \    },\n    \"info\": {\n      \"type\": \"object\",\n      \"description\": \"Match information\",\n      \"properties\": {\n        \"gameCreation\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Unix timestamp when the game was created\"\n        },\n        \"gameDuration\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Game duration in seconds\"\n        },\n        \"gameId\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"gameMode\": {\n          \"type\": \"string\",\n          \"description\": \"Game mode (e.g., CLASSIC, ARAM)\",\n          \"example\": \"CLASSIC\"\n        },\n        \"gameName\": {\n          \"type\": \"string\"\n        },\n        \"gameType\": {\n          \"type\": \"string\",\n          \"description\": \"Game type\",\n          \"example\": \"MATCHED_GAME\"\n        },\n        \"gameVersion\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Patch version\"\n        },\n        \"mapId\": {\n          \"type\": \"integer\",\n          \"description\": \"Map ID\"\n        },\n        \"participants\": {\n          \"type\": \"array\",\n          \"description\": \"Participant data for all 10 players\",\n          \"items\": {\n            \"$ref\": \"#/definitions/Participant\"\n          }\n        },\n        \"platformId\": {\n          \"type\": \"string\",\n          \"description\": \"Platform/region identifier\",\n          \"example\": \"NA1\"\n        },\n        \"queueId\": {\n          \"type\": \"integer\",\n          \"description\": \"Queue type ID\"\n        }\n      }\n    }\n  },\n  \"definitions\": {\n    \"Participant\": {\n      \"type\": \"object\",\n      \"description\": \"A match participant's game data\",\n      \"properties\": {\n        \"puuid\": {\n          \"type\": \"string\"\n        },\n        \"summonerName\": {\n          \"\
  type\": \"string\"\n        },\n        \"championId\": {\n          \"type\": \"integer\"\n        },\n        \"championName\": {\n          \"type\": \"string\"\n        },\n        \"kills\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"deaths\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"assists\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"totalDamageDealt\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\"\n        },\n        \"goldEarned\": {\n          \"type\": \"integer\"\n        },\n        \"win\": {\n          \"type\": \"boolean\"\n        },\n        \"teamId\": {\n          \"type\": \"integer\",\n          \"enum\": [100, 200]\n        },\n        \"teamPosition\": {\n          \"type\": \"string\",\n          \"enum\": [\"TOP\", \"JUNGLE\", \"MIDDLE\", \"BOTTOM\", \"UTILITY\", \"\"]\n        }\n      }\n    }\n  },\n  \"required\"\
  : [\"metadata\", \"info\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/riot-games/refs/heads/main/json-schema/riot-games-match-schema.json
tags:
- Esports
- Gaming
- League of Legends
- Legends of Runeterra
- Teamfight Tactics
- VALORANT
title: Riot Games Match
---
