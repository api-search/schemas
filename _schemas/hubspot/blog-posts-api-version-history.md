---
description: Version history entry for a blog post
layout: schema
name: VersionHistory
properties_list:
- description: Version ID
  name: id
  type: string
- description: Represents a blog post with all content and metadata
  name: object
  type: object
- description: User who made the change
  name: user
  type: object
- description: ISO 8601 timestamp of the version
  name: timestamp
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/blog-posts-api-version-history-schema.json
slug: blog-posts-api-version-history
source_filename: blog-posts-api-version-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-version-history-schema.json\",\n  \"title\": \"VersionHistory\",\n  \"description\": \"Version history entry for a blog post\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Version ID\",\n      \"example\": \"500123\"\n    },\n    \"object\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a blog post with all content and metadata\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the blog post\",\n          \"example\": \"500123\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Internal name of the blog post\",\n          \"example\": \"Example Record\"\n        },\n        \"slug\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"URL slug for the blog post\",\n          \"example\": \"example-value\"\n        },\n        \"htmlTitle\": {\n          \"type\": \"string\",\n          \"description\": \"HTML title tag content\",\n          \"example\": \"Example Record\"\n        },\n        \"postBody\": {\n          \"type\": \"string\",\n          \"description\": \"HTML content of the blog post body\",\n          \"example\": \"This is an example description.\"\n        },\n        \"postSummary\": {\n          \"type\": \"string\",\n          \"description\": \"Summary or excerpt of the blog post\",\n          \"example\": \"example-value\"\n        },\n        \"blogAuthorId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the associated blog author\",\n          \"example\": \"500123\"\n        },\n        \"authorName\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the author\",\n\
  \          \"example\": \"Example Record\"\n        },\n        \"contentGroupId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the blog this post belongs to\",\n          \"example\": \"500123\"\n        },\n        \"campaign\": {\n          \"type\": \"string\",\n          \"description\": \"Campaign GUID associated with the post\",\n          \"example\": \"example-value\"\n        },\n        \"categoryId\": {\n          \"type\": \"integer\",\n          \"description\": \"Category ID for the post\",\n          \"example\": 500123\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"DRAFT\",\n            \"DRAFT_AB\",\n            \"AUTOMATED\",\n            \"PUBLISHED\",\n            \"SCHEDULED\",\n            \"AUTOMATED_DRAFT\"\n          ],\n          \"description\": \"Current state of the blog post\",\n          \"example\": \"DRAFT\"\n        },\n        \"currentState\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Current state description\",\n          \"example\": \"active\"\n        },\n        \"publishDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the post was/will be published\",\n          \"example\": \"2025-03-15T14:30:00Z\"\n        },\n        \"created\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the post was created\",\n          \"example\": \"2025-03-15T14:30:00Z\"\n        },\n        \"updated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the post was last updated\",\n          \"example\": \"2025-03-15T14:30:00Z\"\n        },\n        \"archivedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the post\
  \ was archived\",\n          \"example\": \"2025-03-15T14:30:00Z\"\n        },\n        \"currentlyPublished\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the post is currently published\",\n          \"example\": true\n        },\n        \"domain\": {\n          \"type\": \"string\",\n          \"description\": \"Domain where the post is published\",\n          \"example\": \"example.hubspot.com\"\n        },\n        \"featuredImage\": {\n          \"type\": \"string\",\n          \"description\": \"URL of the featured image\",\n          \"example\": \"example-value\"\n        },\n        \"featuredImageAltText\": {\n          \"type\": \"string\",\n          \"description\": \"Alt text for the featured image\",\n          \"example\": \"example-value\"\n        },\n        \"metaDescription\": {\n          \"type\": \"string\",\n          \"description\": \"Meta description for SEO\",\n          \"example\": \"This is an example description.\"\n    \
  \    },\n        \"headHtml\": {\n          \"type\": \"string\",\n          \"description\": \"Custom HTML for the head section\",\n          \"example\": \"example-value\"\n        },\n        \"footerHtml\": {\n          \"type\": \"string\",\n          \"description\": \"Custom HTML for the footer section\",\n          \"example\": \"example-value\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"Language code of the blog post\",\n          \"example\": \"en\"\n        },\n        \"translatedFromId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the original post this was translated from\",\n          \"example\": \"500123\"\n        },\n        \"tagIds\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"integer\"\n          },\n          \"description\": \"Array of tag IDs associated with the post\",\n          \"example\": [\n            500123\n          ]\n        },\n\
  \        \"useFeaturedImage\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to display the featured image\",\n          \"example\": true\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Full URL of the published post\",\n          \"example\": \"https://app.hubspot.com/contacts/12345\"\n        },\n        \"abStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"master\",\n            \"variant\"\n          ],\n          \"description\": \"A/B test status\",\n          \"example\": \"master\"\n        },\n        \"abTestId\": {\n          \"type\": \"string\",\n          \"description\": \"A/B test ID if part of a test\",\n          \"example\": \"500123\"\n        },\n        \"folderId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the folder containing the post\",\n          \"example\": \"500123\"\n        }\n      },\n\
  \      \"required\": [\n        \"id\",\n        \"name\",\n        \"created\",\n        \"updated\"\n      ]\n    },\n    \"user\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"email\": {\n          \"type\": \"string\"\n        },\n        \"fullName\": {\n          \"type\": \"string\"\n        }\n      },\n      \"description\": \"User who made the change\",\n      \"example\": {\n        \"id\": \"500123\",\n        \"email\": \"jsmith@example.com\",\n        \"fullName\": \"Example Record\"\n      }\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the version\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/blog-posts-api-version-history-schema.json
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
title: VersionHistory
---
