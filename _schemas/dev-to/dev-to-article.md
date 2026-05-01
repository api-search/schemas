---
description: A blog post, discussion, or help thread published on the Dev.to developer community platform. Articles are the primary content type and can include Markdown body text, cover images, tags, and series associations.
layout: schema
name: Dev.to Article
properties_list:
- description: The type of resource, always 'article' for article objects.
  name: type_of
  type: string
- description: The unique numeric identifier of the article.
  name: id
  type: integer
- description: The title of the article.
  name: title
  type: string
- description: A short description or subtitle for the article, typically used for SEO and social sharing.
  name: description
  type: string
- description: The publication date in a human-readable format (e.g., 'Mar 20').
  name: readable_publish_date
  type: string
- description: The URL-friendly slug derived from the article title.
  name: slug
  type: string
- description: The relative path to the article on DEV (e.g., '/username/article-slug-1a2b').
  name: path
  type: string
- description: The full URL of the article on DEV.
  name: url
  type: string
- description: The total number of comments on the article.
  name: comments_count
  type: integer
- description: The total number of public reactions (likes, unicorns, etc.) on the article.
  name: public_reactions_count
  type: integer
- description: The ID of the collection (series) the article belongs to, or null if not part of a series.
  name: collection_id
  type:
  - integer
  - 'null'
- description: The ISO 8601 timestamp when the article was published.
  name: published_timestamp
  type: string
- description: The count of positive reactions on the article.
  name: positive_reactions_count
  type: integer
- description: The URL of the article's cover image, or null if no cover image is set.
  name: cover_image
  type:
  - string
  - 'null'
- description: The URL of the social sharing image generated for the article.
  name: social_image
  type: string
- description: The canonical URL if the article was originally published elsewhere, or the DEV URL.
  name: canonical_url
  type: string
- description: The ISO 8601 timestamp when the article was created.
  name: created_at
  type: string
- description: The ISO 8601 timestamp when the article was last edited, or null if never edited.
  name: edited_at
  type:
  - string
  - 'null'
- description: The ISO 8601 timestamp when the article was crossposted, or null.
  name: crossposted_at
  type:
  - string
  - 'null'
- description: The ISO 8601 timestamp when the article was published.
  name: published_at
  type: string
- description: The ISO 8601 timestamp of the most recent comment, or null if no comments exist.
  name: last_comment_at
  type:
  - string
  - 'null'
- description: The estimated reading time of the article in minutes.
  name: reading_time_minutes
  type: integer
- description: A list of up to four tags associated with the article.
  name: tag_list
  type: array
- description: A comma-separated string of tags associated with the article.
  name: tags
  type: string
- description: The article body rendered as HTML.
  name: body_html
  type: string
- description: The article body in the original Markdown format.
  name: body_markdown
  type: string
- description: Whether the article is currently published.
  name: published
  type: boolean
- description: ''
  name: user
  type: object
- description: ''
  name: organization
  type: object
provider_name: dev-to
provider_slug: dev-to
schema_file: json-schema/dev-to-article-schema.json
slug: dev-to-article
source_filename: dev-to-article-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://dev.to/schemas/dev-to/article.json\",\n  \"title\": \"Dev.to Article\",\n  \"description\": \"A blog post, discussion, or help thread published on the Dev.to developer community platform. Articles are the primary content type and can include Markdown body text, cover images, tags, and series associations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"title\", \"type_of\"],\n  \"properties\": {\n    \"type_of\": {\n      \"type\": \"string\",\n      \"const\": \"article\",\n      \"description\": \"The type of resource, always 'article' for article objects.\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique numeric identifier of the article.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"description\": \"The title of the article.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"A short description or subtitle for the article, typically used for SEO and social sharing.\"\n    },\n    \"readable_publish_date\": {\n      \"type\": \"string\",\n      \"description\": \"The publication date in a human-readable format (e.g., 'Mar 20').\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z0-9]+(?:-[a-z0-9]+)*$\",\n      \"description\": \"The URL-friendly slug derived from the article title.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The relative path to the article on DEV (e.g., '/username/article-slug-1a2b').\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The full URL of the article on DEV.\"\n    },\n    \"comments_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The total number of comments on the article.\"\n    },\n    \"public_reactions_count\": {\n      \"type\":\
  \ \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The total number of public reactions (likes, unicorns, etc.) on the article.\"\n    },\n    \"collection_id\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The ID of the collection (series) the article belongs to, or null if not part of a series.\"\n    },\n    \"published_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the article was published.\"\n    },\n    \"positive_reactions_count\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The count of positive reactions on the article.\"\n    },\n    \"cover_image\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The URL of the article's cover image, or null if no cover image is set.\"\n    },\n    \"social_image\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"The URL of the social sharing image generated for the article.\"\n    },\n    \"canonical_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The canonical URL if the article was originally published elsewhere, or the DEV URL.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the article was created.\"\n    },\n    \"edited_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the article was last edited, or null if never edited.\"\n    },\n    \"crossposted_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the article was crossposted, or null.\"\n    },\n    \"published_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601\
  \ timestamp when the article was published.\"\n    },\n    \"last_comment_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp of the most recent comment, or null if no comments exist.\"\n    },\n    \"reading_time_minutes\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The estimated reading time of the article in minutes.\"\n    },\n    \"tag_list\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"maxItems\": 4,\n      \"description\": \"A list of up to four tags associated with the article.\"\n    },\n    \"tags\": {\n      \"type\": \"string\",\n      \"description\": \"A comma-separated string of tags associated with the article.\"\n    },\n    \"body_html\": {\n      \"type\": \"string\",\n      \"description\": \"The article body rendered as HTML.\"\n    },\n    \"body_markdown\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"The article body in the original Markdown format.\"\n    },\n    \"published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the article is currently published.\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/User\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/$defs/Organization\"\n    }\n  },\n  \"$defs\": {\n    \"User\": {\n      \"type\": \"object\",\n      \"description\": \"The author of the article.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The unique username of the user.\"\n        },\n        \"twitter_username\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The user's Twitter username, or null if not set.\"\n        },\n        \"github_username\": {\n          \"type\": [\"string\", \"\
  null\"],\n          \"description\": \"The user's GitHub username, or null if not set.\"\n        },\n        \"user_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique numeric ID of the user.\"\n        },\n        \"website_url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"The user's website URL, or null if not set.\"\n        },\n        \"location\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The user's location, or null if not set.\"\n        },\n        \"summary\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A brief bio or summary of the user.\"\n        },\n        \"profile_image\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the user's profile image.\"\n        },\n        \"profile_image_90\": {\n          \"type\": \"string\",\n          \"format\":\
  \ \"uri\",\n          \"description\": \"The URL of the 90px profile image.\"\n        },\n        \"joined_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The ISO 8601 timestamp when the user joined the platform.\"\n        }\n      }\n    },\n    \"Organization\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The organization the article was published under, or null if published as an individual.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the organization.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The unique username (slug) of the organization.\"\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"The URL slug of the organization.\"\n        },\n        \"profile_image\": {\n          \"type\": \"string\",\n   \
  \       \"format\": \"uri\",\n          \"description\": \"The URL of the organization's profile image.\"\n        },\n        \"profile_image_90\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the 90px profile image.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/json-schema/dev-to-article-schema.json
tags: []
title: Dev.to Article
---
