---
description: A post resource from the Google Blogger API v3.
layout: schema
name: Blogger Post
properties_list:
- description: ''
  name: kind
  type: string
- description: The identifier of this Post.
  name: id
  type: string
- description: Data about the blog containing this Post.
  name: blog
  type: object
- description: The date the post was published.
  name: published
  type: string
- description: The date the post was last updated.
  name: updated
  type: string
- description: The URL where this Post is displayed.
  name: url
  type: string
- description: The API REST URL to fetch this resource from.
  name: selfLink
  type: string
- description: The title of the Post.
  name: title
  type: string
- description: The content of the Post, which can include HTML markup.
  name: content
  type: string
- description: The author of this Post.
  name: author
  type: object
- description: The list of labels this Post was tagged with.
  name: labels
  type: array
- description: The container of comments on this Post.
  name: replies
  type: object
- description: Status of the post.
  name: status
  type: string
provider_name: Google Blogger
provider_slug: google-blogger
schema_file: json-schema/blogger.json
slug: blogger
source_filename: blogger.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-blogger/refs/heads/main/json-schema/blogger.json\",\n  \"title\": \"Blogger Post\",\n  \"description\": \"A post resource from the Google Blogger API v3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"blogger#post\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of this Post.\"\n    },\n    \"blog\": {\n      \"type\": \"object\",\n      \"description\": \"Data about the blog containing this Post.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"published\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the post was published.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"The date the post was last updated.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL where this Post is displayed.\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API REST URL to fetch this resource from.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Post.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the Post, which can include HTML markup.\"\n    },\n    \"author\": {\n      \"type\": \"object\",\n      \"description\": \"The author of this Post.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"displayName\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"image\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The list of labels this Post was tagged with.\"\n    },\n    \"replies\": {\n      \"type\": \"object\",\n      \"description\": \"The container of comments on this Post.\",\n      \"properties\": {\n        \"totalItems\": {\n          \"type\": \"string\"\n        },\n        \"selfLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"LIVE\", \"DRAFT\", \"SCHEDULED\"],\n      \"description\": \"Status of the post.\"\n    }\n  },\n  \"required\": [\"kind\", \"id\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-blogger/refs/heads/main/json-schema/blogger.json
tags:
- Blogging
- CMS
- Comments
- Google
- Pages
- Posts
- Publishing
title: Blogger Post
---
