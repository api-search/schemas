---
description: A Trello card is the fundamental unit of work on a board. Cards live within lists and can have members, labels, checklists, attachments, due dates, and comments.
layout: schema
name: Trello Card
properties_list:
- description: The unique identifier for the card.
  name: id
  type: string
- description: The name (title) of the card.
  name: name
  type: string
- description: The description of the card, supporting Markdown formatting.
  name: desc
  type: string
- description: Whether the card is archived.
  name: closed
  type: boolean
- description: The ID of the board the card is on.
  name: idBoard
  type: string
- description: The ID of the list the card is in.
  name: idList
  type: string
- description: The short numeric identifier for the card within its board.
  name: idShort
  type: integer
- description: The IDs of members assigned to the card.
  name: idMembers
  type: array
- description: The IDs of labels applied to the card.
  name: idLabels
  type: array
- description: The IDs of checklists on the card.
  name: idChecklists
  type: array
- description: The ID of the attachment used as the card cover image.
  name: idAttachmentCover
  type:
  - string
  - 'null'
- description: The position of the card in its list.
  name: pos
  type: number
- description: The due date for the card.
  name: due
  type:
  - string
  - 'null'
- description: Whether the due date has been marked as complete.
  name: dueComplete
  type: boolean
- description: The start date for the card.
  name: start
  type:
  - string
  - 'null'
- description: The full URL of the card.
  name: url
  type: string
- description: The short URL of the card.
  name: shortUrl
  type: string
- description: The short link identifier for the card.
  name: shortLink
  type: string
- description: Whether the authenticated member is subscribed to the card.
  name: subscribed
  type: boolean
- description: The date and time of the last activity on the card.
  name: dateLastActivity
  type: string
- description: ''
  name: cover
  type: object
- description: The full label objects applied to the card.
  name: labels
  type: array
- description: ''
  name: badges
  type: object
- description: Custom field values set on the card.
  name: customFieldItems
  type: array
provider_name: trello
provider_slug: trello
schema_file: json-schema/trello-card-schema.json
slug: trello-card
source_filename: trello-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://trello.com/schemas/trello/card.json\",\n  \"title\": \"Trello Card\",\n  \"description\": \"A Trello card is the fundamental unit of work on a board. Cards live within lists and can have members, labels, checklists, attachments, due dates, and comments.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"idList\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the card.\",\n      \"pattern\": \"^[0-9a-fA-F]{24}$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name (title) of the card.\",\n      \"maxLength\": 16384\n    },\n    \"desc\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the card, supporting Markdown formatting.\",\n      \"maxLength\": 16384\n    },\n    \"closed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the\
  \ card is archived.\"\n    },\n    \"idBoard\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the board the card is on.\",\n      \"pattern\": \"^[0-9a-fA-F]{24}$\"\n    },\n    \"idList\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the list the card is in.\",\n      \"pattern\": \"^[0-9a-fA-F]{24}$\"\n    },\n    \"idShort\": {\n      \"type\": \"integer\",\n      \"description\": \"The short numeric identifier for the card within its board.\",\n      \"minimum\": 1\n    },\n    \"idMembers\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of members assigned to the card.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[0-9a-fA-F]{24}$\"\n      }\n    },\n    \"idLabels\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of labels applied to the card.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[0-9a-fA-F]{24}$\"\n      }\n    },\n    \"idChecklists\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"The IDs of checklists on the card.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[0-9a-fA-F]{24}$\"\n      }\n    },\n    \"idAttachmentCover\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the attachment used as the card cover image.\",\n      \"pattern\": \"^[0-9a-fA-F]{24}$\"\n    },\n    \"pos\": {\n      \"type\": \"number\",\n      \"description\": \"The position of the card in its list.\"\n    },\n    \"due\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The due date for the card.\"\n    },\n    \"dueComplete\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the due date has been marked as complete.\"\n    },\n    \"start\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The start date for the card.\"\n    },\n    \"url\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The full URL of the card.\"\n    },\n    \"shortUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The short URL of the card.\"\n    },\n    \"shortLink\": {\n      \"type\": \"string\",\n      \"description\": \"The short link identifier for the card.\"\n    },\n    \"subscribed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated member is subscribed to the card.\"\n    },\n    \"dateLastActivity\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the last activity on the card.\"\n    },\n    \"cover\": {\n      \"$ref\": \"#/$defs/CardCover\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"The full label objects applied to the card.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Label\"\n      }\n    },\n    \"badges\": {\n    \
  \  \"$ref\": \"#/$defs/CardBadges\"\n    },\n    \"customFieldItems\": {\n      \"type\": \"array\",\n      \"description\": \"Custom field values set on the card.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomFieldItem\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"CardCover\": {\n      \"type\": \"object\",\n      \"description\": \"The card's cover image or color settings.\",\n      \"properties\": {\n        \"idAttachment\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of the attachment used as the cover.\"\n        },\n        \"color\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The cover color.\"\n        },\n        \"idUploadedBackground\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of an uploaded background used as the cover.\"\n        },\n        \"size\": {\n          \"type\": \"string\",\n          \"description\": \"The size of the cover display.\"\
  ,\n          \"enum\": [\"normal\", \"full\"]\n        },\n        \"brightness\": {\n          \"type\": \"string\",\n          \"description\": \"The brightness of the cover.\",\n          \"enum\": [\"dark\", \"light\"]\n        },\n        \"idPlugin\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of the plugin providing the cover.\"\n        }\n      }\n    },\n    \"CardBadges\": {\n      \"type\": \"object\",\n      \"description\": \"Badge counts and indicators displayed on the card front.\",\n      \"properties\": {\n        \"votes\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of votes on the card.\",\n          \"minimum\": 0\n        },\n        \"attachments\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of attachments on the card.\",\n          \"minimum\": 0\n        },\n        \"comments\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of comments\
  \ on the card.\",\n          \"minimum\": 0\n        },\n        \"checkItems\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of check items across all checklists.\",\n          \"minimum\": 0\n        },\n        \"checkItemsChecked\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of completed check items.\",\n          \"minimum\": 0\n        },\n        \"description\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the card has a description.\"\n        },\n        \"due\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The due date displayed on the badge.\"\n        },\n        \"dueComplete\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the due date is complete.\"\n        },\n        \"subscribed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the member is subscribed.\"\
  \n        },\n        \"start\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The start date for the card.\"\n        }\n      }\n    },\n    \"Label\": {\n      \"type\": \"object\",\n      \"description\": \"A color-coded label applied to a card for categorization.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the label.\",\n          \"pattern\": \"^[0-9a-fA-F]{24}$\"\n        },\n        \"idBoard\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the board the label belongs to.\",\n          \"pattern\": \"^[0-9a-fA-F]{24}$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the label.\"\n        },\n        \"color\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The color of the label.\",\n          \"enum\"\
  : [\"yellow\", \"purple\", \"blue\", \"red\", \"green\", \"orange\", \"black\", \"sky\", \"pink\", \"lime\", null]\n        }\n      }\n    },\n    \"CustomFieldItem\": {\n      \"type\": \"object\",\n      \"description\": \"A custom field value set on a card.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the custom field item.\",\n          \"pattern\": \"^[0-9a-fA-F]{24}$\"\n        },\n        \"idCustomField\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the custom field definition.\",\n          \"pattern\": \"^[0-9a-fA-F]{24}$\"\n        },\n        \"idModel\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the card this value is set on.\",\n          \"pattern\": \"^[0-9a-fA-F]{24}$\"\n        },\n        \"modelType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of model (always 'card').\",\n       \
  \   \"const\": \"card\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"description\": \"The value of the custom field, with a key matching the field type.\",\n          \"properties\": {\n            \"text\": {\n              \"type\": \"string\",\n              \"description\": \"Value for text-type custom fields.\"\n            },\n            \"number\": {\n              \"type\": \"string\",\n              \"description\": \"Value for number-type custom fields (string representation).\"\n            },\n            \"date\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"description\": \"Value for date-type custom fields.\"\n            },\n            \"checked\": {\n              \"type\": \"string\",\n              \"description\": \"Value for checkbox-type custom fields ('true' or 'false').\",\n              \"enum\": [\"true\", \"false\"]\n            }\n          }\n        },\n        \"idValue\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The ID of the selected option for list-type custom fields.\",\n          \"pattern\": \"^[0-9a-fA-F]{24}$\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/json-schema/trello-card-schema.json
tags: []
title: Trello Card
---
