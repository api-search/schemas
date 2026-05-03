---
description: Represents a Reddit comment within a submission's comment tree, including its text content, author information, voting data, and position in the reply hierarchy.
layout: schema
name: Reddit Comment
properties_list:
- description: The unique ID36 identifier for the comment.
  name: id
  type: string
- description: The fullname of the comment, with the t1_ prefix.
  name: name
  type: string
- description: The fullname of the parent thing (t1_ for a comment, t3_ for a submission).
  name: parent_id
  type: string
- description: The fullname of the submission this comment belongs to.
  name: link_id
  type: string
- description: The name of the subreddit this comment was posted in.
  name: subreddit
  type: string
- description: The fullname of the subreddit.
  name: subreddit_id
  type: string
- description: The username of the comment author.
  name: author
  type: string
- description: The fullname of the comment author.
  name: author_fullname
  type: string
- description: The body text of the comment in markdown format.
  name: body
  type: string
- description: The body text of the comment rendered as HTML.
  name: body_html
  type: string
- description: The net score (upvotes minus downvotes) of the comment.
  name: score
  type: integer
- description: The number of upvotes.
  name: ups
  type: integer
- description: The number of downvotes.
  name: downs
  type: integer
- description: The Unix timestamp of when the comment was created.
  name: created_utc
  type: number
- description: The Unix timestamp of the last edit, or false if never edited.
  name: edited
  type:
  - number
  - boolean
- description: Whether the comment author is also the author of the parent submission.
  name: is_submitter
  type: boolean
- description: Whether the comment is stickied (pinned) by a moderator.
  name: stickied
  type: boolean
- description: Whether the comment is locked from replies.
  name: locked
  type: boolean
- description: Whether the comment is archived.
  name: archived
  type: boolean
- description: Whether the comment is saved by the authenticated user.
  name: saved
  type: boolean
- description: Whether the comment has been distinguished by a moderator or admin.
  name: distinguished
  type:
  - string
  - 'null'
- description: The flair text of the comment author in this subreddit.
  name: author_flair_text
  type:
  - string
  - 'null'
- description: The CSS class of the author's flair.
  name: author_flair_css_class
  type:
  - string
  - 'null'
- description: The relative permalink URL of the comment.
  name: permalink
  type: string
- description: The depth of the comment in the reply tree, starting at 0.
  name: depth
  type: integer
- description: The number of times this comment has been gilded.
  name: gilded
  type: integer
- description: The replies to this comment as a Listing object, or an empty string if there are no replies.
  name: replies
  type:
  - object
  - string
- description: Whether the comment score is currently hidden.
  name: score_hidden
  type: boolean
- description: Whether the comment is controversial (0 or 1).
  name: controversiality
  type: integer
provider_name: Reddit
provider_slug: reddit
schema_file: json-schema/reddit-comment-schema.json
slug: reddit-comment
source_filename: reddit-comment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://reddit.com/schemas/reddit/comment.json\",\n  \"title\": \"Reddit Comment\",\n  \"description\": \"Represents a Reddit comment within a submission's comment tree, including its text content, author information, voting data, and position in the reply hierarchy.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"body\", \"author\", \"link_id\", \"created_utc\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID36 identifier for the comment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The fullname of the comment, with the t1_ prefix.\",\n      \"pattern\": \"^t1_[a-z0-9]+$\"\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"description\": \"The fullname of the parent thing (t1_ for a comment, t3_ for a submission).\",\n      \"pattern\": \"^t[13]_[a-z0-9]+$\"\n    },\n\
  \    \"link_id\": {\n      \"type\": \"string\",\n      \"description\": \"The fullname of the submission this comment belongs to.\",\n      \"pattern\": \"^t3_[a-z0-9]+$\"\n    },\n    \"subreddit\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the subreddit this comment was posted in.\"\n    },\n    \"subreddit_id\": {\n      \"type\": \"string\",\n      \"description\": \"The fullname of the subreddit.\",\n      \"pattern\": \"^t5_[a-z0-9]+$\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the comment author.\"\n    },\n    \"author_fullname\": {\n      \"type\": \"string\",\n      \"description\": \"The fullname of the comment author.\",\n      \"pattern\": \"^t2_[a-z0-9]+$\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The body text of the comment in markdown format.\"\n    },\n    \"body_html\": {\n      \"type\": \"string\",\n      \"description\": \"The body text of the\
  \ comment rendered as HTML.\"\n    },\n    \"score\": {\n      \"type\": \"integer\",\n      \"description\": \"The net score (upvotes minus downvotes) of the comment.\"\n    },\n    \"ups\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of upvotes.\"\n    },\n    \"downs\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of downvotes.\"\n    },\n    \"created_utc\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The Unix timestamp of when the comment was created.\"\n    },\n    \"edited\": {\n      \"type\": [\"number\", \"boolean\"],\n      \"description\": \"The Unix timestamp of the last edit, or false if never edited.\"\n    },\n    \"is_submitter\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the comment author is also the author of the parent submission.\"\n    },\n    \"stickied\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the comment is stickied (pinned)\
  \ by a moderator.\"\n    },\n    \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the comment is locked from replies.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the comment is archived.\"\n    },\n    \"saved\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the comment is saved by the authenticated user.\"\n    },\n    \"distinguished\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Whether the comment has been distinguished by a moderator or admin.\",\n      \"enum\": [null, \"moderator\", \"admin\"]\n    },\n    \"author_flair_text\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The flair text of the comment author in this subreddit.\"\n    },\n    \"author_flair_css_class\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The CSS class of the author's flair.\"\n    },\n    \"permalink\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The relative permalink URL of the comment.\"\n    },\n    \"depth\": {\n      \"type\": \"integer\",\n      \"description\": \"The depth of the comment in the reply tree, starting at 0.\",\n      \"minimum\": 0\n    },\n    \"gilded\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times this comment has been gilded.\",\n      \"minimum\": 0\n    },\n    \"replies\": {\n      \"type\": [\"object\", \"string\"],\n      \"description\": \"The replies to this comment as a Listing object, or an empty string if there are no replies.\"\n    },\n    \"score_hidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the comment score is currently hidden.\"\n    },\n    \"controversiality\": {\n      \"type\": \"integer\",\n      \"description\": \"Whether the comment is controversial (0 or 1).\",\n      \"minimum\": 0,\n      \"maximum\": 1\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/json-schema/reddit-comment-schema.json
tags:
- Advertising
- Communities
- Content
- Social Media
- Social News
title: Reddit Comment
---
