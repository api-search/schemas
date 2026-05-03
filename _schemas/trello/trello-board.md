---
description: A Trello board is the primary organizational unit containing lists and cards. Boards belong to organizations (workspaces) and have members with varying permission levels.
layout: schema
name: Trello Board
properties_list:
- description: The unique identifier for the board.
  name: id
  type: string
- description: The name of the board.
  name: name
  type: string
- description: The description of the board.
  name: desc
  type: string
- description: Additional structured description data.
  name: descData
  type:
  - object
  - 'null'
- description: Whether the board is closed (archived).
  name: closed
  type: boolean
- description: The ID of the member who created the board.
  name: idMemberCreator
  type: string
- description: The ID of the organization (workspace) the board belongs to.
  name: idOrganization
  type:
  - string
  - 'null'
- description: Whether the board is pinned.
  name: pinned
  type: boolean
- description: The full URL of the board on trello.com.
  name: url
  type: string
- description: The short URL of the board.
  name: shortUrl
  type: string
- description: The short link identifier for the board.
  name: shortLink
  type: string
- description: Whether the authenticated member has starred the board.
  name: starred
  type: boolean
- description: The date and time of the last activity on the board.
  name: dateLastActivity
  type:
  - string
  - 'null'
- description: The date and time the authenticated member last viewed the board.
  name: dateLastView
  type:
  - string
  - 'null'
- description: ''
  name: prefs
  type: object
- description: ''
  name: labelNames
  type: object
- description: The board's membership records.
  name: memberships
  type: array
provider_name: trello
provider_slug: trello
schema_file: json-schema/trello-board-schema.json
slug: trello-board
source_filename: trello-board-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://trello.com/schemas/trello/board.json\",\n  \"title\": \"Trello Board\",\n  \"description\": \"A Trello board is the primary organizational unit containing lists and cards. Boards belong to organizations (workspaces) and have members with varying permission levels.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the board.\",\n      \"pattern\": \"^[0-9a-fA-F]{24}$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the board.\",\n      \"minLength\": 1,\n      \"maxLength\": 16384\n    },\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the board.\",\n      \"maxLength\": 16384\n    },\n    \"descData\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"\
  Additional structured description data.\"\n    },\n    \"closed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the board is closed (archived).\"\n    },\n    \"idMemberCreator\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the member who created the board.\",\n      \"pattern\": \"^[0-9a-fA-F]{24}$\"\n    },\n    \"idOrganization\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the organization (workspace) the board belongs to.\",\n      \"pattern\": \"^[0-9a-fA-F]{24}$\"\n    },\n    \"pinned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the board is pinned.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The full URL of the board on trello.com.\"\n    },\n    \"shortUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The short URL of the board.\"\n    },\n    \"shortLink\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The short link identifier for the board.\"\n    },\n    \"starred\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated member has starred the board.\"\n    },\n    \"dateLastActivity\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the last activity on the board.\"\n    },\n    \"dateLastView\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the authenticated member last viewed the board.\"\n    },\n    \"prefs\": {\n      \"$ref\": \"#/$defs/BoardPrefs\"\n    },\n    \"labelNames\": {\n      \"$ref\": \"#/$defs/LabelNames\"\n    },\n    \"memberships\": {\n      \"type\": \"array\",\n      \"description\": \"The board's membership records.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Membership\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"BoardPrefs\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Board preferences and configuration settings.\",\n      \"properties\": {\n        \"permissionLevel\": {\n          \"type\": \"string\",\n          \"description\": \"The visibility/permission level of the board.\",\n          \"enum\": [\"org\", \"private\", \"public\"]\n        },\n        \"hideVotes\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether votes are hidden until voting is complete.\"\n        },\n        \"voting\": {\n          \"type\": \"string\",\n          \"description\": \"Who can vote on cards on the board.\",\n          \"enum\": [\"disabled\", \"members\", \"observers\", \"org\", \"public\"]\n        },\n        \"comments\": {\n          \"type\": \"string\",\n          \"description\": \"Who can comment on cards on the board.\",\n          \"enum\": [\"disabled\", \"members\", \"observers\", \"org\", \"public\"]\n        },\n        \"selfJoin\": {\n          \"type\": \"boolean\"\
  ,\n          \"description\": \"Whether workspace members can join the board themselves.\"\n        },\n        \"cardCovers\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether card cover images are enabled.\"\n        },\n        \"cardAging\": {\n          \"type\": \"string\",\n          \"description\": \"The card aging style applied to the board.\",\n          \"enum\": [\"pirate\", \"regular\"]\n        },\n        \"calendarFeedEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the calendar feed is enabled.\"\n        },\n        \"background\": {\n          \"type\": \"string\",\n          \"description\": \"The background identifier (color name or image ID).\"\n        },\n        \"backgroundColor\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The background color hex code.\"\n        },\n        \"backgroundImage\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\"\
  : \"uri\",\n          \"description\": \"The URL of the background image.\"\n        },\n        \"backgroundTile\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the background image is tiled.\"\n        },\n        \"backgroundBrightness\": {\n          \"type\": \"string\",\n          \"description\": \"The brightness level of the background.\",\n          \"enum\": [\"dark\", \"light\", \"unknown\"]\n        }\n      }\n    },\n    \"LabelNames\": {\n      \"type\": \"object\",\n      \"description\": \"The names assigned to each label color on the board.\",\n      \"properties\": {\n        \"green\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the green label.\"\n        },\n        \"yellow\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the yellow label.\"\n        },\n        \"orange\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the orange label.\"\n        },\n\
  \        \"red\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the red label.\"\n        },\n        \"purple\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the purple label.\"\n        },\n        \"blue\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the blue label.\"\n        },\n        \"sky\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the sky label.\"\n        },\n        \"lime\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the lime label.\"\n        },\n        \"pink\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the pink label.\"\n        },\n        \"black\": {\n          \"type\": \"string\",\n          \"description\": \"Name for the black label.\"\n        }\n      }\n    },\n    \"Membership\": {\n      \"type\": \"object\",\n      \"description\": \"A membership record linking a member to the\
  \ board with a specific role.\",\n      \"required\": [\"id\", \"idMember\", \"memberType\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the membership.\",\n          \"pattern\": \"^[0-9a-fA-F]{24}$\"\n        },\n        \"idMember\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the member.\",\n          \"pattern\": \"^[0-9a-fA-F]{24}$\"\n        },\n        \"memberType\": {\n          \"type\": \"string\",\n          \"description\": \"The role of the member on the board.\",\n          \"enum\": [\"admin\", \"normal\", \"observer\"]\n        },\n        \"unconfirmed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the membership invitation is unconfirmed.\"\n        },\n        \"deactivated\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the membership is deactivated.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/json-schema/trello-board-schema.json
tags: []
title: Trello Board
---
