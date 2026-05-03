---
description: A video game entry in the RAWG database with metadata including platforms, ratings, genres, and social data.
layout: schema
name: RAWG Game
properties_list:
- description: Unique integer identifier for the game
  name: id
  type: integer
- description: URL-safe slug identifier for the game
  name: slug
  type: string
- description: Primary display name of the game
  name: name
  type: string
- description: Original name of the game (may differ from localized name)
  name: name_original
  type: string
- description: Full description of the game
  name: description
  type: string
- description: Official release date of the game
  name: released
  type: string
- description: Whether the game is marked as To Be Announced
  name: tba
  type: boolean
- description: Last updated timestamp for this game record
  name: updated
  type: string
- description: URL to the primary background image
  name: background_image
  type: string
- description: URL to an additional background image
  name: background_image_additional
  type: string
- description: Official website URL for the game
  name: website
  type: string
- description: Average community rating (0-5 scale)
  name: rating
  type: number
- description: Maximum possible rating
  name: rating_top
  type: integer
- description: Breakdown of rating distribution
  name: ratings
  type: object
- description: Total number of ratings received
  name: ratings_count
  type: integer
- description: Number of text reviews
  name: reviews_text_count
  type: string
- description: Number of users who have added this game to their collection
  name: added
  type: integer
- description: Breakdown of users by library status (owned, played, etc.)
  name: added_by_status
  type: object
- description: Metacritic score (0-100)
  name: metacritic
  type: integer
- description: Average playtime in hours
  name: playtime
  type: integer
- description: Number of screenshots available
  name: screenshots_count
  type: integer
- description: Number of trailers/movies available
  name: movies_count
  type: integer
- description: Number of credited creators
  name: creators_count
  type: integer
- description: Number of achievements
  name: achievements_count
  type: integer
- description: Number of similar game suggestions
  name: suggestions_count
  type: integer
- description: URL to the game's subreddit
  name: reddit_url
  type: string
- description: Name of the game's subreddit
  name: reddit_name
  type: string
- description: Number of parent games (for DLCs/editions)
  name: parents_count
  type: integer
- description: Number of DLCs and additions
  name: additions_count
  type: integer
- description: Number of games in the same series
  name: game_series_count
  type: integer
- description: List of alternative names or regional titles
  name: alternative_names
  type: array
- description: URL to the game's Metacritic page
  name: metacritic_url
  type: string
- description: ''
  name: esrb_rating
  type: object
- description: List of platforms the game is available on
  name: platforms
  type: array
provider_name: RAWG
provider_slug: rawg
schema_file: json-schema/rawg-game-schema.json
slug: rawg-game
source_filename: rawg-game-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/rawg/refs/heads/main/json-schema/rawg-game-schema.json\",\n  \"title\": \"RAWG Game\",\n  \"description\": \"A video game entry in the RAWG database with metadata including platforms, ratings, genres, and social data.\",\n  \"type\": \"object\",\n  \"required\": [\"rating\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique integer identifier for the game\",\n      \"readOnly\": true\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-safe slug identifier for the game\",\n      \"pattern\": \"^[-a-zA-Z0-9_]+$\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Primary display name of the game\",\n      \"readOnly\": true\n    },\n    \"name_original\": {\n      \"type\": \"string\",\n      \"description\": \"Original\
  \ name of the game (may differ from localized name)\",\n      \"readOnly\": true\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full description of the game\",\n      \"readOnly\": true\n    },\n    \"released\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Official release date of the game\",\n      \"readOnly\": true\n    },\n    \"tba\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the game is marked as To Be Announced\",\n      \"readOnly\": true\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last updated timestamp for this game record\",\n      \"readOnly\": true\n    },\n    \"background_image\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the primary background image\",\n      \"readOnly\": true\n    },\n    \"background_image_additional\": {\n      \"type\": \"\
  string\",\n      \"description\": \"URL to an additional background image\",\n      \"readOnly\": true\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Official website URL for the game\",\n      \"readOnly\": true\n    },\n    \"rating\": {\n      \"type\": \"number\",\n      \"description\": \"Average community rating (0-5 scale)\",\n      \"minimum\": 0,\n      \"maximum\": 5\n    },\n    \"rating_top\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum possible rating\",\n      \"readOnly\": true\n    },\n    \"ratings\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of rating distribution\",\n      \"readOnly\": true\n    },\n    \"ratings_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of ratings received\",\n      \"readOnly\": true\n    },\n    \"reviews_text_count\": {\n      \"type\": \"string\",\n      \"description\": \"Number of text reviews\"\
  ,\n      \"readOnly\": true\n    },\n    \"added\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of users who have added this game to their collection\",\n      \"readOnly\": true\n    },\n    \"added_by_status\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of users by library status (owned, played, etc.)\",\n      \"readOnly\": true\n    },\n    \"metacritic\": {\n      \"type\": \"integer\",\n      \"description\": \"Metacritic score (0-100)\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"readOnly\": true\n    },\n    \"playtime\": {\n      \"type\": \"integer\",\n      \"description\": \"Average playtime in hours\",\n      \"readOnly\": true\n    },\n    \"screenshots_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of screenshots available\",\n      \"readOnly\": true\n    },\n    \"movies_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of trailers/movies available\",\n      \"\
  readOnly\": true\n    },\n    \"creators_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of credited creators\",\n      \"readOnly\": true\n    },\n    \"achievements_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of achievements\",\n      \"readOnly\": true\n    },\n    \"suggestions_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of similar game suggestions\",\n      \"readOnly\": true\n    },\n    \"reddit_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the game's subreddit\",\n      \"readOnly\": true\n    },\n    \"reddit_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the game's subreddit\",\n      \"readOnly\": true\n    },\n    \"parents_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of parent games (for DLCs/editions)\",\n      \"readOnly\": true\n    },\n    \"additions_count\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Number of DLCs and additions\",\n      \"readOnly\": true\n    },\n    \"game_series_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of games in the same series\",\n      \"readOnly\": true\n    },\n    \"alternative_names\": {\n      \"type\": \"array\",\n      \"description\": \"List of alternative names or regional titles\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true\n    },\n    \"metacritic_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the game's Metacritic page\",\n      \"readOnly\": true\n    },\n    \"esrb_rating\": {\n      \"$ref\": \"#/definitions/EsrbRating\"\n    },\n    \"platforms\": {\n      \"type\": \"array\",\n      \"description\": \"List of platforms the game is available on\",\n      \"items\": {\n        \"$ref\": \"#/definitions/GamePlatformEntry\"\n      }\n    }\n  },\n  \"definitions\": {\n    \"EsrbRating\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"ESRB content rating classification\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"enum\": [\"everyone\", \"everyone-10-plus\", \"teen\", \"mature\", \"adults-only\", \"rating-pending\"]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"enum\": [\"Everyone\", \"Everyone 10+\", \"Teen\", \"Mature\", \"Adults Only\", \"Rating Pending\"]\n        }\n      }\n    },\n    \"PlatformRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a gaming platform\",\n      \"properties\": {\n        \"id\": {\"type\": \"integer\"},\n        \"slug\": {\"type\": \"string\"},\n        \"name\": {\"type\": \"string\"}\n      }\n    },\n    \"PlatformRequirements\": {\n      \"type\": \"object\",\n      \"description\": \"System requirements for a platform\",\n      \"properties\": {\n        \"minimum\": {\"type\": \"string\"},\n        \"\
  recommended\": {\"type\": \"string\"}\n      }\n    },\n    \"GamePlatformEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A platform entry with release date and system requirements\",\n      \"properties\": {\n        \"platform\": {\"$ref\": \"#/definitions/PlatformRef\"},\n        \"released_at\": {\"type\": \"string\", \"nullable\": true},\n        \"requirements\": {\"$ref\": \"#/definitions/PlatformRequirements\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rawg/refs/heads/main/json-schema/rawg-game-schema.json
tags:
- Database
- Entertainment
- Game Discovery
- Games
- Gaming
- Metadata
- Video Games
title: RAWG Game
---
