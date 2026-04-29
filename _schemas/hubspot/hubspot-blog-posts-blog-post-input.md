---
description: Input data for creating or updating a blog post
layout: schema
name: BlogPostInput
properties_list:
- description: Internal name of the blog post
  name: name
  type: string
- description: URL slug for the blog post
  name: slug
  type: string
- description: HTML title tag content
  name: htmlTitle
  type: string
- description: HTML content of the blog post body
  name: postBody
  type: string
- description: Summary or excerpt of the blog post
  name: postSummary
  type: string
- description: ID of the associated blog author
  name: blogAuthorId
  type: string
- description: ID of the blog this post belongs to
  name: contentGroupId
  type: string
- description: Campaign GUID
  name: campaign
  type: string
- description: Scheduled publish date
  name: publishDate
  type: string
- description: URL of the featured image
  name: featuredImage
  type: string
- description: Alt text for the featured image
  name: featuredImageAltText
  type: string
- description: Meta description for SEO
  name: metaDescription
  type: string
- description: Tag IDs to associate
  name: tagIds
  type: array
- description: Whether to display the featured image
  name: useFeaturedImage
  type: boolean
- description: Language code
  name: language
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-blog-posts-blog-post-input-schema.json
slug: hubspot-blog-posts-blog-post-input
source_filename: hubspot-blog-posts-blog-post-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Input data for creating or updating a blog post\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the blog post\",\n      \"example\": \"Example Record\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL slug for the blog post\",\n      \"example\": \"example-value\"\n    },\n    \"htmlTitle\": {\n      \"type\": \"string\",\n      \"description\": \"HTML title tag content\",\n      \"example\": \"Example Record\"\n    },\n    \"postBody\": {\n      \"type\": \"string\",\n      \"description\": \"HTML content of the blog post body\",\n      \"example\": \"This is an example description.\"\n    },\n    \"postSummary\": {\n      \"type\": \"string\",\n      \"description\": \"Summary or excerpt of the blog post\",\n      \"example\": \"example-value\"\n    },\n    \"blogAuthorId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"ID of the associated blog author\",\n      \"example\": \"500123\"\n    },\n    \"contentGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the blog this post belongs to\",\n      \"example\": \"500123\"\n    },\n    \"campaign\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign GUID\",\n      \"example\": \"example-value\"\n    },\n    \"publishDate\": {\n      \"type\": \"string\",\n      \"description\": \"Scheduled publish date\",\n      \"format\": \"date-time\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"featuredImage\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the featured image\",\n      \"example\": \"example-value\"\n    },\n    \"featuredImageAltText\": {\n      \"type\": \"string\",\n      \"description\": \"Alt text for the featured image\",\n      \"example\": \"example-value\"\n    },\n    \"metaDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Meta description for SEO\"\
  ,\n      \"example\": \"This is an example description.\"\n    },\n    \"tagIds\": {\n      \"type\": \"array\",\n      \"description\": \"Tag IDs to associate\",\n      \"example\": [\n        500123\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"useFeaturedImage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to display the featured image\",\n      \"example\": true\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code\",\n      \"example\": \"en\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"contentGroupId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlogPostInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-blog-posts-blog-post-input-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: BlogPostInput
---
