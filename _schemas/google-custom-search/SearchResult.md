---
description: A search result returned by the Google Custom Search JSON API.
layout: schema
name: Google Custom Search Result
properties_list:
- description: The kind of result.
  name: kind
  type: string
- description: The title of the search result.
  name: title
  type: string
- description: The title with HTML formatting.
  name: htmlTitle
  type: string
- description: The URL of the search result.
  name: link
  type: string
- description: An abridged version of the URL.
  name: displayLink
  type: string
- description: A snippet of the search result.
  name: snippet
  type: string
- description: The snippet with HTML formatting.
  name: htmlSnippet
  type: string
- description: The cache ID for Google's cached version.
  name: cacheId
  type: string
- description: The formatted URL.
  name: formattedUrl
  type: string
- description: The formatted URL with HTML formatting.
  name: htmlFormattedUrl
  type: string
- description: PageMap information for the result.
  name: pagemap
  type: object
- description: The MIME type of the result.
  name: mime
  type: string
- description: The file format of the result.
  name: fileFormat
  type: string
- description: Image information if this is an image result.
  name: image
  type: object
provider_name: Google Custom Search
provider_slug: google-custom-search
schema_file: json-schema/SearchResult.json
slug: SearchResult
source_filename: SearchResult.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"SearchResult.json\",\n  \"title\": \"Google Custom Search Result\",\n  \"description\": \"A search result returned by the Google Custom Search JSON API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of result.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the search result.\"\n    },\n    \"htmlTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The title with HTML formatting.\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the search result.\"\n    },\n    \"displayLink\": {\n      \"type\": \"string\",\n      \"description\": \"An abridged version of the URL.\"\n    },\n    \"snippet\": {\n      \"type\": \"string\",\n      \"description\": \"A snippet of the search result.\"\
  \n    },\n    \"htmlSnippet\": {\n      \"type\": \"string\",\n      \"description\": \"The snippet with HTML formatting.\"\n    },\n    \"cacheId\": {\n      \"type\": \"string\",\n      \"description\": \"The cache ID for Google's cached version.\"\n    },\n    \"formattedUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The formatted URL.\"\n    },\n    \"htmlFormattedUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The formatted URL with HTML formatting.\"\n    },\n    \"pagemap\": {\n      \"type\": \"object\",\n      \"description\": \"PageMap information for the result.\"\n    },\n    \"mime\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the result.\"\n    },\n    \"fileFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The file format of the result.\"\n    },\n    \"image\": {\n      \"type\": \"object\",\n      \"description\": \"Image information if this is an image result.\",\n      \"properties\": {\n\
  \        \"contextLink\": {\n          \"type\": \"string\"\n        },\n        \"height\": {\n          \"type\": \"integer\"\n        },\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"byteSize\": {\n          \"type\": \"integer\"\n        },\n        \"thumbnailLink\": {\n          \"type\": \"string\"\n        },\n        \"thumbnailHeight\": {\n          \"type\": \"integer\"\n        },\n        \"thumbnailWidth\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-custom-search/refs/heads/main/json-schema/SearchResult.json
tags:
- Custom Search
- Google
- Image Search
- Search
- Web Search
title: Google Custom Search Result
---
