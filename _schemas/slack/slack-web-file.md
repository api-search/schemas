---
description: A Slack file object representing an uploaded file with its metadata and sharing information.
layout: schema
name: File
properties_list:
- description: Unique file identifier.
  name: id
  type: string
- description: Unix timestamp of when the file was created.
  name: created
  type: integer
- description: Unix timestamp.
  name: timestamp
  type: integer
- description: The file name.
  name: name
  type: string
- description: Title of the file.
  name: title
  type: string
- description: MIME type of the file.
  name: mimetype
  type: string
- description: Slack file type identifier (e.g., "png", "pdf", "snippet").
  name: filetype
  type: string
- description: Human-readable file type.
  name: pretty_type
  type: string
- description: User ID of the user who uploaded the file.
  name: user
  type: string
- description: Team ID of the user who uploaded the file.
  name: user_team
  type: string
- description: Whether the file content is editable.
  name: editable
  type: boolean
- description: File size in bytes.
  name: size
  type: integer
- description: File mode (e.g., "hosted", "external", "snippet", "post").
  name: mode
  type: string
- description: Whether the file is externally hosted.
  name: is_external
  type: boolean
- description: Type of external file.
  name: external_type
  type: string
- description: Whether the file is public.
  name: is_public
  type: boolean
- description: ''
  name: public_url_shared
  type: boolean
- description: ''
  name: display_as_bot
  type: boolean
- description: ''
  name: username
  type: string
- description: URL to access the file. Requires authentication.
  name: url_private
  type: string
- description: URL to download the file. Requires authentication.
  name: url_private_download
  type: string
- description: Permalink URL for the file.
  name: permalink
  type: string
- description: Public permalink URL for the file (if shared publicly).
  name: permalink_public
  type: string
- description: Array of channel IDs where the file is shared.
  name: channels
  type: array
- description: Array of private channel IDs where the file is shared.
  name: groups
  type: array
- description: Array of DM IDs where the file is shared.
  name: ims
  type: array
- description: Sharing information broken down by type.
  name: shares
  type: object
- description: Number of comments on the file.
  name: comments_count
  type: integer
provider_name: Slack
provider_slug: slack
schema_file: json-schema/slack-web-file-schema.json
slug: slack-web-file
source_filename: slack-web-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"File\",\n  \"type\": \"object\",\n  \"description\": \"A Slack file object representing an uploaded file with its metadata and sharing information.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique file identifier.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the file was created.\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The file name.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the file.\"\n    },\n    \"mimetype\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the file.\"\n    },\n    \"filetype\": {\n      \"type\": \"string\",\n      \"description\": \"Slack file\
  \ type identifier (e.g., \\\"png\\\", \\\"pdf\\\", \\\"snippet\\\").\"\n    },\n    \"pretty_type\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable file type.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the user who uploaded the file.\"\n    },\n    \"user_team\": {\n      \"type\": \"string\",\n      \"description\": \"Team ID of the user who uploaded the file.\"\n    },\n    \"editable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the file content is editable.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"File size in bytes.\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"File mode (e.g., \\\"hosted\\\", \\\"external\\\", \\\"snippet\\\", \\\"post\\\").\"\n    },\n    \"is_external\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the file is externally hosted.\"\n    },\n    \"external_type\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Type of external file.\"\n    },\n    \"is_public\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the file is public.\"\n    },\n    \"public_url_shared\": {\n      \"type\": \"boolean\"\n    },\n    \"display_as_bot\": {\n      \"type\": \"boolean\"\n    },\n    \"username\": {\n      \"type\": \"string\"\n    },\n    \"url_private\": {\n      \"type\": \"string\",\n      \"description\": \"URL to access the file. Requires authentication.\"\n    },\n    \"url_private_download\": {\n      \"type\": \"string\",\n      \"description\": \"URL to download the file. Requires authentication.\"\n    },\n    \"permalink\": {\n      \"type\": \"string\",\n      \"description\": \"Permalink URL for the file.\"\n    },\n    \"permalink_public\": {\n      \"type\": \"string\",\n      \"description\": \"Public permalink URL for the file (if shared publicly).\"\n    },\n    \"channels\": {\n      \"type\": \"array\",\n      \"\
  description\": \"Array of channel IDs where the file is shared.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"Array of private channel IDs where the file is shared.\"\n    },\n    \"ims\": {\n      \"type\": \"array\",\n      \"description\": \"Array of DM IDs where the file is shared.\"\n    },\n    \"shares\": {\n      \"type\": \"object\",\n      \"description\": \"Sharing information broken down by type.\"\n    },\n    \"comments_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of comments on the file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/json-schema/slack-web-file-schema.json
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
title: File
---
