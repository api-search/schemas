---
description: A comment on a review, changelist, or other topic in Helix Swarm.
layout: schema
name: Comment
properties_list:
- description: The unique comment identifier.
  name: id
  type: integer
- description: File attachments on the comment.
  name: attachments
  type: array
- description: The comment body text.
  name: body
  type: string
- description: Inline context for file-level comments.
  name: context
  type: object
- description: Unix timestamp of the last edit, or null if not edited.
  name: edited
  type: integer
- description: Flags applied to the comment.
  name: flags
  type: array
- description: Usernames of users who liked the comment.
  name: likes
  type: array
- description: The task state of the comment.
  name: taskState
  type: string
- description: Unix timestamp when the comment was created.
  name: time
  type: integer
- description: The topic the comment belongs to, such as reviews/1234.
  name: topic
  type: string
- description: Unix timestamp of the last update.
  name: updated
  type: integer
- description: The username of the comment author.
  name: user
  type: string
provider_name: Perforce
provider_slug: perforce
schema_file: json-schema/perforce-helix-swarm-comment-schema.json
slug: perforce-helix-swarm-comment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment\",\n  \"type\": \"object\",\n  \"description\": \"A comment on a review, changelist, or other topic in Helix Swarm.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique comment identifier.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"File attachments on the comment.\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The comment body text.\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Inline context for file-level comments.\"\n    },\n    \"edited\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the last edit, or null if not edited.\"\n    },\n    \"flags\": {\n      \"type\": \"array\",\n      \"description\": \"Flags applied to the comment.\"\n    },\n    \"likes\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Usernames of users who liked the comment.\"\n    },\n    \"taskState\": {\n      \"type\": \"string\",\n      \"description\": \"The task state of the comment.\"\n    },\n    \"time\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp when the comment was created.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"The topic the comment belongs to, such as reviews/1234.\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the last update.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the comment author.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/json-schema/perforce-helix-swarm-comment-schema.json
tags: []
title: Comment
---
