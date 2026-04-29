---
description: Information about a sitemap submitted to Search Console. Includes processing status, error counts, and content details.
layout: schema
name: WmxSitemap
properties_list:
- description: The URL of the sitemap.
  name: path
  type: string
- description: Date and time when the sitemap was last submitted to Search Console.
  name: lastSubmitted
  type: string
- description: Whether the sitemap is still being processed.
  name: isPending
  type: boolean
- description: Whether this is a sitemap index file.
  name: isSitemapsIndex
  type: boolean
- description: The type of content in the sitemap.
  name: type
  type: string
- description: Date and time when the sitemap was last downloaded by Google.
  name: lastDownloaded
  type: string
- description: Number of warnings for the sitemap.
  name: warnings
  type: integer
- description: Number of errors for the sitemap.
  name: errors
  type: integer
- description: Content details for this sitemap, broken down by content type.
  name: contents
  type: array
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-wmx-sitemap-schema.json
slug: google-search-console-wmx-sitemap
source_filename: google-search-console-wmx-sitemap-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WmxSitemap\",\n  \"type\": \"object\",\n  \"description\": \"Information about a sitemap submitted to Search Console. Includes processing status, error counts, and content details.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the sitemap.\"\n    },\n    \"lastSubmitted\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the sitemap was last submitted to Search Console.\"\n    },\n    \"isPending\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the sitemap is still being processed.\"\n    },\n    \"isSitemapsIndex\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a sitemap index file.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of content in the sitemap.\"\n    },\n    \"lastDownloaded\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Date and time when the sitemap was last downloaded by Google.\"\n    },\n    \"warnings\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of warnings for the sitemap.\"\n    },\n    \"errors\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of errors for the sitemap.\"\n    },\n    \"contents\": {\n      \"type\": \"array\",\n      \"description\": \"Content details for this sitemap, broken down by content type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-wmx-sitemap-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: WmxSitemap
---
