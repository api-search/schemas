---
description: A post represents a piece of content in a Ghost publication, including blog posts and newsletter content. Posts support rich content via the Lexical editor format, SEO metadata, social sharing metadata, content visibility controls, and associations with authors and tags.
layout: schema
name: Ghost Post
properties_list:
- description: Unique identifier for the post
  name: id
  type: string
- description: Universally unique identifier for the post
  name: uuid
  type: string
- description: Title of the post
  name: title
  type: string
- description: URL-safe slug derived from the title, used in the post URL
  name: slug
  type: string
- description: Post content in Lexical editor format, stored as a JSON string
  name: lexical
  type: string
- description: Rendered HTML content of the post
  name: html
  type: string
- description: Plain text representation of the post content
  name: plaintext
  type: string
- description: Identifier used by the commenting system
  name: comment_id
  type: string
- description: URL of the featured image displayed at the top of the post
  name: feature_image
  type:
  - string
  - 'null'
- description: Alt text for the featured image for accessibility
  name: feature_image_alt
  type:
  - string
  - 'null'
- description: Caption displayed below the featured image
  name: feature_image_caption
  type:
  - string
  - 'null'
- description: Whether the post is marked as featured for prominent display
  name: featured
  type: boolean
- description: Publication status of the post
  name: status
  type: string
- description: Controls which audience can access the full post content
  name: visibility
  type: string
- description: ISO 8601 timestamp when the post was created
  name: created_at
  type: string
- description: ISO 8601 timestamp when the post was last updated, required for edit operations to prevent collisions
  name: updated_at
  type: string
- description: ISO 8601 timestamp when the post was published or is scheduled to be published
  name: published_at
  type:
  - string
  - 'null'
- description: Custom excerpt to override the auto-generated excerpt
  name: custom_excerpt
  type:
  - string
  - 'null'
- description: Custom code injected into the HTML head on the post page
  name: codeinjection_head
  type:
  - string
  - 'null'
- description: Custom code injected before the closing body tag on the post page
  name: codeinjection_foot
  type:
  - string
  - 'null'
- description: Name of a custom Handlebars template to use for rendering the post
  name: custom_template
  type:
  - string
  - 'null'
- description: Canonical URL for the post, used when content is syndicated from another source
  name: canonical_url
  type:
  - string
  - 'null'
- description: Full URL of the post on the Ghost site
  name: url
  type: string
- description: Auto-generated excerpt from the beginning of the post content
  name: excerpt
  type: string
- description: Estimated reading time in minutes based on word count
  name: reading_time
  type: integer
- description: Whether the current request has access to the full post content based on visibility settings
  name: access
  type: boolean
- description: Custom subject line when sending the post as a newsletter email
  name: email_subject
  type:
  - string
  - 'null'
- description: Custom frontmatter data for the post
  name: frontmatter
  type:
  - string
  - 'null'
- description: Open Graph image URL used when the post is shared on social platforms
  name: og_image
  type:
  - string
  - 'null'
- description: Open Graph title for social sharing
  name: og_title
  type:
  - string
  - 'null'
- description: Open Graph description for social sharing
  name: og_description
  type:
  - string
  - 'null'
- description: Twitter card image URL
  name: twitter_image
  type:
  - string
  - 'null'
- description: Twitter card title
  name: twitter_title
  type:
  - string
  - 'null'
- description: Twitter card description
  name: twitter_description
  type:
  - string
  - 'null'
- description: Custom SEO meta title for search engine results
  name: meta_title
  type:
  - string
  - 'null'
- description: Custom SEO meta description for search engine results
  name: meta_description
  type:
  - string
  - 'null'
- description: Tags associated with the post for categorization
  name: tags
  type: array
- description: Authors of the post, at least one author is always present
  name: authors
  type: array
- description: The primary (first) author of the post
  name: primary_author
  type: object
- description: The primary (first) tag of the post
  name: primary_tag
  type: object
provider_name: Ghost
provider_slug: ghost
schema_file: json-schema/ghost-post-schema.json
slug: ghost-post
source_filename: ghost-post-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://ghost.org/schemas/ghost/post.json\",\n  \"title\": \"Ghost Post\",\n  \"description\": \"A post represents a piece of content in a Ghost publication, including blog posts and newsletter content. Posts support rich content via the Lexical editor format, SEO metadata, social sharing metadata, content visibility controls, and associations with authors and tags.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"title\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the post\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Universally unique identifier for the post\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the post\",\n      \"minLength\": 1,\n      \"maxLength\": 2000\n    },\n\
  \    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-safe slug derived from the title, used in the post URL\",\n      \"pattern\": \"^[a-z0-9]+(?:-[a-z0-9]+)*$\",\n      \"maxLength\": 191\n    },\n    \"lexical\": {\n      \"type\": \"string\",\n      \"description\": \"Post content in Lexical editor format, stored as a JSON string\"\n    },\n    \"html\": {\n      \"type\": \"string\",\n      \"description\": \"Rendered HTML content of the post\"\n    },\n    \"plaintext\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text representation of the post content\"\n    },\n    \"comment_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier used by the commenting system\"\n    },\n    \"feature_image\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL of the featured image displayed at the top of the post\"\n    },\n    \"feature_image_alt\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"description\": \"Alt text for the featured image for accessibility\",\n      \"maxLength\": 191\n    },\n    \"feature_image_caption\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Caption displayed below the featured image\"\n    },\n    \"featured\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is marked as featured for prominent display\",\n      \"default\": false\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Publication status of the post\",\n      \"enum\": [\"published\", \"draft\", \"scheduled\", \"sent\"],\n      \"default\": \"draft\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Controls which audience can access the full post content\",\n      \"enum\": [\"public\", \"members\", \"paid\", \"tiers\"],\n      \"default\": \"public\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"ISO 8601 timestamp when the post was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the post was last updated, required for edit operations to prevent collisions\"\n    },\n    \"published_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the post was published or is scheduled to be published\"\n    },\n    \"custom_excerpt\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Custom excerpt to override the auto-generated excerpt\",\n      \"maxLength\": 300\n    },\n    \"codeinjection_head\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Custom code injected into the HTML head on the post page\"\n    },\n    \"codeinjection_foot\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Custom code injected before the closing body tag on the\
  \ post page\"\n    },\n    \"custom_template\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of a custom Handlebars template to use for rendering the post\"\n    },\n    \"canonical_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Canonical URL for the post, used when content is syndicated from another source\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Full URL of the post on the Ghost site\"\n    },\n    \"excerpt\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated excerpt from the beginning of the post content\"\n    },\n    \"reading_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Estimated reading time in minutes based on word count\",\n      \"minimum\": 0\n    },\n    \"access\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current request has access to the full post content\
  \ based on visibility settings\"\n    },\n    \"email_subject\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Custom subject line when sending the post as a newsletter email\"\n    },\n    \"frontmatter\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Custom frontmatter data for the post\"\n    },\n    \"og_image\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Open Graph image URL used when the post is shared on social platforms\"\n    },\n    \"og_title\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Open Graph title for social sharing\",\n      \"maxLength\": 300\n    },\n    \"og_description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Open Graph description for social sharing\",\n      \"maxLength\": 500\n    },\n    \"twitter_image\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Twitter\
  \ card image URL\"\n    },\n    \"twitter_title\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Twitter card title\",\n      \"maxLength\": 300\n    },\n    \"twitter_description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Twitter card description\",\n      \"maxLength\": 500\n    },\n    \"meta_title\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Custom SEO meta title for search engine results\",\n      \"maxLength\": 300\n    },\n    \"meta_description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Custom SEO meta description for search engine results\",\n      \"maxLength\": 500\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the post for categorization\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    },\n    \"authors\": {\n      \"type\": \"array\",\n      \"description\": \"Authors of the post, at least one\
  \ author is always present\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Author\"\n      },\n      \"minItems\": 1\n    },\n    \"primary_author\": {\n      \"$ref\": \"#/$defs/Author\",\n      \"description\": \"The primary (first) author of the post\"\n    },\n    \"primary_tag\": {\n      \"description\": \"The primary (first) tag of the post\",\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/Tag\" },\n        { \"type\": \"null\" }\n      ]\n    }\n  },\n  \"$defs\": {\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A tag for organizing and categorizing content in Ghost\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the tag\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the tag\",\n          \"minLength\": 1,\n          \"maxLength\"\
  : 191\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"URL-safe slug for the tag\",\n          \"pattern\": \"^[a-z0-9]+(?:-[a-z0-9]+)*$\",\n          \"maxLength\": 191\n        },\n        \"description\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Description of the tag\",\n          \"maxLength\": 500\n        },\n        \"feature_image\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"Featured image URL for the tag page\"\n        },\n        \"visibility\": {\n          \"type\": \"string\",\n          \"description\": \"Visibility of the tag, internal tags have slugs starting with hash\",\n          \"enum\": [\"public\", \"internal\"]\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Full URL of the tag page\"\n        }\n      }\n    },\n    \"Author\": {\n  \
  \    \"type\": \"object\",\n      \"description\": \"A staff user who creates content in the Ghost publication\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the author\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the author\"\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"URL-safe slug for the author\",\n          \"maxLength\": 191\n        },\n        \"profile_image\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"Profile image URL\"\n        },\n        \"cover_image\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"Cover image URL for the author page\"\n        },\n        \"bio\": {\n\
  \          \"type\": [\"string\", \"null\"],\n          \"description\": \"Author biography\",\n          \"maxLength\": 200\n        },\n        \"website\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"Author personal website URL\"\n        },\n        \"location\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Author location\",\n          \"maxLength\": 150\n        },\n        \"facebook\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Facebook username\"\n        },\n        \"twitter\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Twitter handle\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Full URL of the author page\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/json-schema/ghost-post-schema.json
tags:
- Content Management
- Publishing
- Headless CMS
- Blogging
- Newsletters
- Memberships
title: Ghost Post
---
