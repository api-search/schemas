---
description: A League of Legends summoner profile from the Riot Games API
layout: schema
name: Riot Games Summoner
properties_list:
- description: Encrypted summoner ID (region-specific)
  name: id
  type: string
- description: Encrypted account ID (region-specific)
  name: accountId
  type: string
- description: Encrypted PUUID (globally unique, use for cross-game lookups)
  name: puuid
  type: string
- description: Summoner name (deprecated, use Riot ID gameName+tagLine)
  name: name
  type: string
- description: Profile icon ID, resolvable via Data Dragon
  name: profileIconId
  type: integer
- description: Unix timestamp of last profile update
  name: revisionDate
  type: integer
- description: Summoner level
  name: summonerLevel
  type: integer
provider_name: Riot Games
provider_slug: riot-games
schema_file: json-schema/riot-games-summoner-schema.json
slug: riot-games-summoner
source_filename: riot-games-summoner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/riot-games/blob/main/json-schema/riot-games-summoner-schema.json\",\n  \"title\": \"Riot Games Summoner\",\n  \"description\": \"A League of Legends summoner profile from the Riot Games API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Encrypted summoner ID (region-specific)\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Encrypted account ID (region-specific)\"\n    },\n    \"puuid\": {\n      \"type\": \"string\",\n      \"description\": \"Encrypted PUUID (globally unique, use for cross-game lookups)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Summoner name (deprecated, use Riot ID gameName+tagLine)\"\n    },\n    \"profileIconId\": {\n      \"type\": \"integer\",\n      \"description\": \"Profile icon ID, resolvable\
  \ via Data Dragon\"\n    },\n    \"revisionDate\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix timestamp of last profile update\"\n    },\n    \"summonerLevel\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Summoner level\",\n      \"minimum\": 1\n    }\n  },\n  \"required\": [\"id\", \"puuid\", \"summonerLevel\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/riot-games/refs/heads/main/json-schema/riot-games-summoner-schema.json
tags:
- Esports
- Gaming
- League of Legends
- Legends of Runeterra
- Teamfight Tactics
- VALORANT
title: Riot Games Summoner
---
