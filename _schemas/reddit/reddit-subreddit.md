---
description: Represents a Reddit subreddit community, including its display configuration, subscriber count, rules, and moderation settings.
layout: schema
name: Reddit Subreddit
properties_list:
- description: The unique ID36 identifier for the subreddit.
  name: id
  type: string
- description: The fullname of the subreddit, with the t5_ prefix.
  name: name
  type: string
- description: The display name of the subreddit without the r/ prefix.
  name: display_name
  type: string
- description: The display name with the r/ prefix.
  name: display_name_prefixed
  type: string
- description: The title of the subreddit shown in the header.
  name: title
  type: string
- description: A short public description shown in search results and listings.
  name: public_description
  type: string
- description: The full sidebar description in markdown format.
  name: description
  type: string
- description: The sidebar description rendered as HTML.
  name: description_html
  type:
  - string
  - 'null'
- description: The total number of subscribers.
  name: subscribers
  type: integer
- description: The approximate number of users currently active in the subreddit.
  name: accounts_active
  type:
  - integer
  - 'null'
- description: The Unix timestamp of when the subreddit was created.
  name: created_utc
  type: number
- description: The access type of the subreddit.
  name: subreddit_type
  type: string
- description: The types of submissions allowed.
  name: submission_type
  type: string
- description: The primary language of the subreddit (IETF language tag).
  name: lang
  type: string
- description: Whether the subreddit is marked as NSFW.
  name: over18
  type: boolean
- description: Whether spoiler tagging is enabled.
  name: spoilers_enabled
  type: boolean
- description: Whether image posts are allowed.
  name: allow_images
  type: boolean
- description: Whether video posts are allowed.
  name: allow_videos
  type: boolean
- description: Whether poll posts are allowed.
  name: allow_polls
  type: boolean
- description: The relative URL path of the subreddit.
  name: url
  type: string
- description: The URL of the subreddit icon image.
  name: icon_img
  type: string
- description: The URL of the subreddit banner image.
  name: banner_img
  type: string
- description: The URL of the subreddit header image.
  name: header_img
  type:
  - string
  - 'null'
- description: The URL of the community icon.
  name: community_icon
  type: string
- description: The primary theme color as a hex code.
  name: primary_color
  type: string
- description: The key accent color as a hex code.
  name: key_color
  type: string
- description: Whether the subreddit wiki is enabled.
  name: wiki_enabled
  type:
  - boolean
  - 'null'
- description: Whether the authenticated user is subscribed to this subreddit.
  name: user_is_subscriber
  type:
  - boolean
  - 'null'
- description: Whether the authenticated user is a moderator of this subreddit.
  name: user_is_moderator
  type:
  - boolean
  - 'null'
- description: Whether the authenticated user is banned from this subreddit.
  name: user_is_banned
  type:
  - boolean
  - 'null'
provider_name: Reddit
provider_slug: reddit
schema_file: json-schema/reddit-subreddit-schema.json
slug: reddit-subreddit
source_filename: reddit-subreddit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://reddit.com/schemas/reddit/subreddit.json\",\n  \"title\": \"Reddit Subreddit\",\n  \"description\": \"Represents a Reddit subreddit community, including its display configuration, subscriber count, rules, and moderation settings.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"display_name\", \"title\", \"created_utc\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID36 identifier for the subreddit.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The fullname of the subreddit, with the t5_ prefix.\",\n      \"pattern\": \"^t5_[a-z0-9]+$\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the subreddit without the r/ prefix.\"\n    },\n    \"display_name_prefixed\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The display name with the r/ prefix.\",\n      \"pattern\": \"^r/\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the subreddit shown in the header.\"\n    },\n    \"public_description\": {\n      \"type\": \"string\",\n      \"description\": \"A short public description shown in search results and listings.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The full sidebar description in markdown format.\"\n    },\n    \"description_html\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The sidebar description rendered as HTML.\"\n    },\n    \"subscribers\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of subscribers.\",\n      \"minimum\": 0\n    },\n    \"accounts_active\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The approximate number of users currently active in the subreddit.\"\n    },\n    \"created_utc\": {\n \
  \     \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The Unix timestamp of when the subreddit was created.\"\n    },\n    \"subreddit_type\": {\n      \"type\": \"string\",\n      \"description\": \"The access type of the subreddit.\",\n      \"enum\": [\"public\", \"private\", \"restricted\", \"gold_restricted\", \"archived\"]\n    },\n    \"submission_type\": {\n      \"type\": \"string\",\n      \"description\": \"The types of submissions allowed.\",\n      \"enum\": [\"any\", \"link\", \"self\"]\n    },\n    \"lang\": {\n      \"type\": \"string\",\n      \"description\": \"The primary language of the subreddit (IETF language tag).\"\n    },\n    \"over18\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the subreddit is marked as NSFW.\"\n    },\n    \"spoilers_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether spoiler tagging is enabled.\"\n    },\n    \"allow_images\": {\n      \"type\": \"boolean\",\n\
  \      \"description\": \"Whether image posts are allowed.\"\n    },\n    \"allow_videos\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether video posts are allowed.\"\n    },\n    \"allow_polls\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether poll posts are allowed.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The relative URL path of the subreddit.\"\n    },\n    \"icon_img\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the subreddit icon image.\"\n    },\n    \"banner_img\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the subreddit banner image.\"\n    },\n    \"header_img\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URL of the subreddit header image.\"\n    },\n    \"community_icon\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n     \
  \ \"description\": \"The URL of the community icon.\"\n    },\n    \"primary_color\": {\n      \"type\": \"string\",\n      \"description\": \"The primary theme color as a hex code.\",\n      \"pattern\": \"^#[0-9a-fA-F]{6}$\"\n    },\n    \"key_color\": {\n      \"type\": \"string\",\n      \"description\": \"The key accent color as a hex code.\",\n      \"pattern\": \"^#[0-9a-fA-F]{6}$\"\n    },\n    \"wiki_enabled\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the subreddit wiki is enabled.\"\n    },\n    \"user_is_subscriber\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the authenticated user is subscribed to this subreddit.\"\n    },\n    \"user_is_moderator\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the authenticated user is a moderator of this subreddit.\"\n    },\n    \"user_is_banned\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether the authenticated\
  \ user is banned from this subreddit.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/json-schema/reddit-subreddit-schema.json
tags:
- Advertising
- Communities
- Content
- Social Media
- Social News
title: Reddit Subreddit
---
