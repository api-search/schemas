---
description: The schema for a single search result returned by the Fumadocs search API endpoint. Each result represents a matched documentation segment at page, heading, or text granularity. Results include the page URL, matched content with optional highlight markers, and breadcrumbs for navigation context.
layout: schema
name: Fumadocs Search Result
properties_list:
- description: Unique identifier for this search result within the index. Used by the client for result deduplication and React key assignment.
  name: id
  type: string
- description: Relative URL path of the documentation page containing this result. May include a fragment identifier pointing to a specific heading anchor.
  name: url
  type: string
- description: Granularity level of the matched content. 'page' indicates the page title matched; 'heading' indicates a section heading matched; 'text' indicates body paragraph text matched.
  name: type
  type: string
- description: The matched text content. May contain inline Markdown highlight annotations using <mark> tags wrapping the matched query terms to enable client-side highlight rendering.
  name: content
  type: string
- description: 'Ordered list of ancestor section and page titles forming the breadcrumb trail to this result. Displayed in the search results UI to give users navigation context for where the result lives within the '
  name: breadcrumbs
  type: array
provider_name: Fumadocs
provider_slug: fumadocs
schema_file: json-schema/fumadocs-search-result-schema.json
slug: fumadocs-search-result
source_filename: fumadocs-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fumadocs.dev/schemas/search-result.json\",\n  \"title\": \"Fumadocs Search Result\",\n  \"description\": \"The schema for a single search result returned by the Fumadocs search API endpoint. Each result represents a matched documentation segment at page, heading, or text granularity. Results include the page URL, matched content with optional highlight markers, and breadcrumbs for navigation context.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"url\", \"type\", \"content\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this search result within the index. Used by the client for result deduplication and React key assignment.\",\n      \"example\": \"docs/getting-started#installation\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL path of the documentation page containing\
  \ this result. May include a fragment identifier pointing to a specific heading anchor.\",\n      \"example\": \"/docs/getting-started#installation\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Granularity level of the matched content. 'page' indicates the page title matched; 'heading' indicates a section heading matched; 'text' indicates body paragraph text matched.\",\n      \"enum\": [\"page\", \"heading\", \"text\"]\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The matched text content. May contain inline Markdown highlight annotations using <mark> tags wrapping the matched query terms to enable client-side highlight rendering.\",\n      \"example\": \"Install Fumadocs using your preferred package manager\"\n    },\n    \"breadcrumbs\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of ancestor section and page titles forming the breadcrumb trail to this result. Displayed in the search results\
  \ UI to give users navigation context for where the result lives within the documentation.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"A breadcrumb label for an ancestor page or section.\"\n      },\n      \"example\": [\"Documentation\", \"Getting Started\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fumadocs/refs/heads/main/json-schema/fumadocs-search-result-schema.json
tags:
- Documentation
- Framework
- Next.js
- React
title: Fumadocs Search Result
---
