---
description: Hearthstone metadata including sets, classes, keywords, types, and rarities.
layout: schema
name: Metadata
properties_list:
- description: List of card sets.
  name: sets
  type: array
- description: List of set groups.
  name: setGroups
  type: array
- description: List of classes.
  name: classes
  type: array
- description: List of keywords.
  name: keywords
  type: array
- description: List of card types.
  name: types
  type: array
- description: List of rarities.
  name: rarities
  type: array
- description: List of minion types.
  name: minionTypes
  type: array
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-metadata-schema.json
slug: hearthstone-game-data-metadata
source_filename: hearthstone-game-data-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-metadata-schema.json\",\n  \"title\": \"Metadata\",\n  \"description\": \"Hearthstone metadata including sets, classes, keywords, types, and rarities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique ID of the metadata item.\",\n            \"example\": 1\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the metadata item.\",\n            \"example\": \"Basic\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"The slug identifier.\",\n            \"\
  example\": \"basic\"\n          }\n        },\n        \"description\": \"A generic metadata item.\"\n      },\n      \"description\": \"List of card sets.\"\n    },\n    \"setGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique ID of the metadata item.\",\n            \"example\": 1\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the metadata item.\",\n            \"example\": \"Basic\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"The slug identifier.\",\n            \"example\": \"basic\"\n          }\n        },\n        \"description\": \"A generic metadata item.\"\n      },\n      \"description\": \"List of set groups.\"\n    },\n    \"classes\": {\n      \"type\": \"array\",\n      \"items\":\
  \ {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique ID of the metadata item.\",\n            \"example\": 1\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the metadata item.\",\n            \"example\": \"Basic\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"The slug identifier.\",\n            \"example\": \"basic\"\n          }\n        },\n        \"description\": \"A generic metadata item.\"\n      },\n      \"description\": \"List of classes.\"\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique ID of the metadata item.\",\n            \"example\": 1\n          },\n  \
  \        \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the metadata item.\",\n            \"example\": \"Basic\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"The slug identifier.\",\n            \"example\": \"basic\"\n          }\n        },\n        \"description\": \"A generic metadata item.\"\n      },\n      \"description\": \"List of keywords.\"\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique ID of the metadata item.\",\n            \"example\": 1\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the metadata item.\",\n            \"example\": \"Basic\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n      \
  \      \"description\": \"The slug identifier.\",\n            \"example\": \"basic\"\n          }\n        },\n        \"description\": \"A generic metadata item.\"\n      },\n      \"description\": \"List of card types.\"\n    },\n    \"rarities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique ID of the metadata item.\",\n            \"example\": 1\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the metadata item.\",\n            \"example\": \"Basic\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"The slug identifier.\",\n            \"example\": \"basic\"\n          }\n        },\n        \"description\": \"A generic metadata item.\"\n      },\n      \"description\": \"List of rarities.\"\n    },\n \
  \   \"minionTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique ID of the metadata item.\",\n            \"example\": 1\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the metadata item.\",\n            \"example\": \"Basic\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"The slug identifier.\",\n            \"example\": \"basic\"\n          }\n        },\n        \"description\": \"A generic metadata item.\"\n      },\n      \"description\": \"List of minion types.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-metadata-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: Metadata
---
