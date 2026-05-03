---
description: Represents a Reddit submission (also known as a post or link), including its content, metadata, voting data, and associated subreddit information.
layout: schema
name: Reddit Post (Submission)
properties_list:
- description: The unique ID36 identifier for the post.
  name: id
  type: string
- description: The fullname of the post, with the t3_ prefix.
  name: name
  type: string
- description: The name of the subreddit the post was submitted to, without the r/ prefix.
  name: subreddit
  type: string
- description: The fullname of the subreddit.
  name: subreddit_id
  type: string
- description: The title of the post.
  name: title
  type: string
- description: The username of the post author.
  name: author
  type: string
- description: The fullname of the post author.
  name: author_fullname
  type: string
- description: The body text of a self-post in markdown format. Empty string for link posts.
  name: selftext
  type: string
- description: The body text of a self-post rendered as HTML.
  name: selftext_html
  type:
  - string
  - 'null'
- description: The URL of the linked content, or the permalink for self-posts.
  name: url
  type: string
- description: The relative permalink URL of the post on Reddit.
  name: permalink
  type: string
- description: The domain of the linked URL.
  name: domain
  type: string
- description: Whether the post is a self-post (text post) rather than a link post.
  name: is_self
  type: boolean
- description: Whether the post contains hosted video content.
  name: is_video
  type: boolean
- description: The net score (upvotes minus downvotes) of the post.
  name: score
  type: integer
- description: The number of upvotes.
  name: ups
  type: integer
- description: The number of downvotes.
  name: downs
  type: integer
- description: The ratio of upvotes to total votes, between 0.0 and 1.0.
  name: upvote_ratio
  type: number
- description: The number of comments on the post.
  name: num_comments
  type: integer
- description: The Unix timestamp of when the post was created.
  name: created_utc
  type: number
- description: The Unix timestamp of the last edit, or false if never edited.
  name: edited
  type:
  - number
  - boolean
- description: Whether the post is marked as NSFW.
  name: over_18
  type: boolean
- description: Whether the post is marked as a spoiler.
  name: spoiler
  type: boolean
- description: Whether the post is stickied (pinned) in the subreddit.
  name: stickied
  type: boolean
- description: Whether the post is locked from new comments.
  name: locked
  type: boolean
- description: Whether the post is archived and no longer accepts votes or comments.
  name: archived
  type: boolean
- description: Whether the post is hidden by the authenticated user.
  name: hidden
  type: boolean
- description: Whether the post is saved by the authenticated user.
  name: saved
  type: boolean
- description: Whether the post has been distinguished by a moderator or admin.
  name: distinguished
  type:
  - string
  - 'null'
- description: The text of the link flair applied to the post.
  name: link_flair_text
  type:
  - string
  - 'null'
- description: The CSS class of the link flair.
  name: link_flair_css_class
  type:
  - string
  - 'null'
- description: The URL of the post thumbnail, or a placeholder value like self, default, image, or nsfw.
  name: thumbnail
  type: string
- description: The width of the thumbnail in pixels.
  name: thumbnail_width
  type:
  - integer
  - 'null'
- description: The height of the thumbnail in pixels.
  name: thumbnail_height
  type:
  - integer
  - 'null'
- description: Media metadata for video or embedded content posts.
  name: media
  type:
  - object
  - 'null'
- description: The number of times this post has been gilded (awarded gold).
  name: gilded
  type: integer
- description: The number of times this post has been crossposted.
  name: num_crossposts
  type: integer
provider_name: Reddit
provider_slug: reddit
schema_file: json-schema/reddit-post-schema.json
slug: reddit-post
source_filename: reddit-post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://reddit.com/schemas/reddit/post.json\",\n  \"title\": \"Reddit Post (Submission)\",\n  \"description\": \"Represents a Reddit submission (also known as a post or link), including its content, metadata, voting data, and associated subreddit information.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"subreddit\", \"title\", \"author\", \"created_utc\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique ID36 identifier for the post.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The fullname of the post, with the t3_ prefix.\",\n      \"pattern\": \"^t3_[a-z0-9]+$\"\n    },\n    \"subreddit\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the subreddit the post was submitted to, without the r/ prefix.\"\n    },\n    \"subreddit_id\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The fullname of the subreddit.\",\n      \"pattern\": \"^t5_[a-z0-9]+$\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the post.\",\n      \"maxLength\": 300\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the post author.\"\n    },\n    \"author_fullname\": {\n      \"type\": \"string\",\n      \"description\": \"The fullname of the post author.\",\n      \"pattern\": \"^t2_[a-z0-9]+$\"\n    },\n    \"selftext\": {\n      \"type\": \"string\",\n      \"description\": \"The body text of a self-post in markdown format. Empty string for link posts.\"\n    },\n    \"selftext_html\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The body text of a self-post rendered as HTML.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the linked content, or the permalink for self-posts.\"\
  \n    },\n    \"permalink\": {\n      \"type\": \"string\",\n      \"description\": \"The relative permalink URL of the post on Reddit.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain of the linked URL.\"\n    },\n    \"is_self\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is a self-post (text post) rather than a link post.\"\n    },\n    \"is_video\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post contains hosted video content.\"\n    },\n    \"score\": {\n      \"type\": \"integer\",\n      \"description\": \"The net score (upvotes minus downvotes) of the post.\"\n    },\n    \"ups\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of upvotes.\"\n    },\n    \"downs\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of downvotes.\"\n    },\n    \"upvote_ratio\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\"\
  : \"The ratio of upvotes to total votes, between 0.0 and 1.0.\",\n      \"minimum\": 0.0,\n      \"maximum\": 1.0\n    },\n    \"num_comments\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of comments on the post.\",\n      \"minimum\": 0\n    },\n    \"created_utc\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The Unix timestamp of when the post was created.\"\n    },\n    \"edited\": {\n      \"type\": [\"number\", \"boolean\"],\n      \"description\": \"The Unix timestamp of the last edit, or false if never edited.\"\n    },\n    \"over_18\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is marked as NSFW.\"\n    },\n    \"spoiler\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is marked as a spoiler.\"\n    },\n    \"stickied\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is stickied (pinned) in the subreddit.\"\n    },\n   \
  \ \"locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is locked from new comments.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is archived and no longer accepts votes or comments.\"\n    },\n    \"hidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is hidden by the authenticated user.\"\n    },\n    \"saved\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is saved by the authenticated user.\"\n    },\n    \"distinguished\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Whether the post has been distinguished by a moderator or admin.\",\n      \"enum\": [null, \"moderator\", \"admin\"]\n    },\n    \"link_flair_text\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The text of the link flair applied to the post.\"\n    },\n    \"link_flair_css_class\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"description\": \"The CSS class of the link flair.\"\n    },\n    \"thumbnail\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the post thumbnail, or a placeholder value like self, default, image, or nsfw.\"\n    },\n    \"thumbnail_width\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The width of the thumbnail in pixels.\"\n    },\n    \"thumbnail_height\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The height of the thumbnail in pixels.\"\n    },\n    \"media\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Media metadata for video or embedded content posts.\"\n    },\n    \"gilded\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times this post has been gilded (awarded gold).\",\n      \"minimum\": 0\n    },\n    \"num_crossposts\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times this post has been crossposted.\",\n    \
  \  \"minimum\": 0\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/json-schema/reddit-post-schema.json
tags:
- Advertising
- Communities
- Content
- Social Media
- Social News
title: Reddit Post (Submission)
---
