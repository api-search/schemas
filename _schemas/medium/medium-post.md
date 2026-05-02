---
description: A post published on the Medium platform, including its content metadata, publishing status, tags, licensing, and authorship details.
layout: schema
name: Medium Post
properties_list:
- description: The unique identifier assigned to the post by Medium.
  name: id
  type: string
- description: The title of the post, limited to 100 characters.
  name: title
  type: string
- description: The format of the content field, either HTML or Markdown.
  name: contentFormat
  type: string
- description: The body content of the post in the format specified by contentFormat.
  name: content
  type: string
- description: The unique identifier of the user who authored the post.
  name: authorId
  type: string
- description: Tags to classify the post, limited to a maximum of three tags with each up to 25 characters.
  name: tags
  type: array
- description: The original URL if this post was first published elsewhere, used for SEO canonical linking.
  name: canonicalUrl
  type: string
- description: The publish status of the post. Public posts are visible to everyone, drafts are private, and unlisted posts are accessible only via direct link.
  name: publishStatus
  type: string
- description: The timestamp in milliseconds when the post was published.
  name: publishedAt
  type: integer
- description: The license under which the post is published.
  name: license
  type: string
- description: The URL to the full text of the license under which the post is published.
  name: licenseUrl
  type: string
- description: The URL to the post on Medium.
  name: url
  type: string
- description: The unique identifier of the publication the post belongs to, if published within a publication.
  name: publicationId
  type: string
- description: Whether to notify the author's followers about the new post.
  name: notifyFollowers
  type: boolean
provider_name: medium
provider_slug: medium
schema_file: json-schema/medium-post-schema.json
slug: medium-post
source_filename: medium-post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://medium.com/schemas/medium/post.json\",\n  \"title\": \"Medium Post\",\n  \"description\": \"A post published on the Medium platform, including its content metadata, publishing status, tags, licensing, and authorship details.\",\n  \"type\": \"object\",\n  \"required\": [\"title\", \"contentFormat\", \"content\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the post by Medium.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"The title of the post, limited to 100 characters.\"\n    },\n    \"contentFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\"html\", \"markdown\"],\n      \"description\": \"The format of the content field, either HTML or Markdown.\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n\
  \      \"description\": \"The body content of the post in the format specified by contentFormat.\"\n    },\n    \"authorId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the user who authored the post.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"maxItems\": 3,\n      \"items\": {\n        \"type\": \"string\",\n        \"maxLength\": 25\n      },\n      \"description\": \"Tags to classify the post, limited to a maximum of three tags with each up to 25 characters.\"\n    },\n    \"canonicalUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The original URL if this post was first published elsewhere, used for SEO canonical linking.\"\n    },\n    \"publishStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"draft\", \"unlisted\"],\n      \"default\": \"public\",\n      \"description\": \"The publish status of the post. Public posts are visible to everyone, drafts are private,\
  \ and unlisted posts are accessible only via direct link.\"\n    },\n    \"publishedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The timestamp in milliseconds when the post was published.\"\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"all-rights-reserved\",\n        \"cc-40-by\",\n        \"cc-40-by-sa\",\n        \"cc-40-by-nd\",\n        \"cc-40-by-nc\",\n        \"cc-40-by-nc-nd\",\n        \"cc-40-by-nc-sa\",\n        \"cc-40-zero\",\n        \"public-domain\"\n      ],\n      \"default\": \"all-rights-reserved\",\n      \"description\": \"The license under which the post is published.\"\n    },\n    \"licenseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the full text of the license under which the post is published.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the\
  \ post on Medium.\"\n    },\n    \"publicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the publication the post belongs to, if published within a publication.\"\n    },\n    \"notifyFollowers\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to notify the author's followers about the new post.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/json-schema/medium-post-schema.json
tags: []
title: Medium Post
---
