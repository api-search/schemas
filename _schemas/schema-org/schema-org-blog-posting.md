---
description: A blog post. A subtype of Article and SocialMediaPosting.
layout: schema
name: Schema.org BlogPosting
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: Headline of the blog post.
  name: headline
  type: string
- description: The name of the blog post.
  name: name
  type: string
- description: A short description of the blog post.
  name: description
  type: string
- description: The actual body of the blog post.
  name: articleBody
  type: string
- description: URL of the blog post.
  name: url
  type: string
- description: An image for the blog post.
  name: image
  type: object
- description: The author of this blog post.
  name: author
  type: object
- description: The publisher of this blog post.
  name: publisher
  type: object
- description: Date of first publication.
  name: datePublished
  type: string
- description: The date on which the blog post was created.
  name: dateCreated
  type: string
- description: The date on which the blog post was most recently modified.
  name: dateModified
  type: string
- description: Keywords or tags.
  name: keywords
  type: object
- description: The number of words in the text.
  name: wordCount
  type: integer
- description: The language of the content.
  name: inLanguage
  type: string
- description: A CreativeWork such as an image, video, or audio clip shared as part of this posting.
  name: sharedContent
  type: object
- description: Indicates a page for which this blog post is the main entity.
  name: mainEntityOfPage
  type: object
- description: The number of comments this blog post has received.
  name: commentCount
  type: integer
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-blog-posting-schema.json
slug: schema-org-blog-posting
source_filename: schema-org-blog-posting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/blog-posting.json\",\n  \"title\": \"Schema.org BlogPosting\",\n  \"description\": \"A blog post. A subtype of Article and SocialMediaPosting.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"headline\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"BlogPosting\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"headline\": {\n      \"type\": \"string\",\n      \"maxLength\": 110,\n      \"description\": \"Headline of the blog post.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the blog post.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the blog post.\"\n    },\n    \"articleBody\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"The actual body of the blog post.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the blog post.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image for the blog post.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The author of this blog post.\"\n    },\n    \"publisher\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The publisher of this blog post.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n     \
  \ \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date on which the blog post was created.\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date on which the blog post was most recently modified.\"\n    },\n    \"keywords\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Keywords or tags.\"\n    },\n    \"wordCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of words in the text.\"\n    },\n    \"inLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the content.\"\n    },\n    \"sharedContent\": {\n      \"type\": \"object\",\n      \"description\": \"A CreativeWork such as an image, video, or\
  \ audio clip shared as part of this posting.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    },\n    \"mainEntityOfPage\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-web-page-schema.json\" }\n      ],\n      \"description\": \"Indicates a page for which this blog post is the main entity.\"\n    },\n    \"commentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of comments this blog post has received.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-blog-posting-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org BlogPosting
---
