---
description: JSON Schema representing the structure of Google News RSS feed items.
layout: schema
name: Google News RSS Feed Schema
properties_list: []
provider_name: Google News RSS
provider_slug: google-news
schema_file: json-schema/google-news.json
slug: google-news
source_filename: google-news.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-news/refs/heads/main/json-schema/google-news.json\",\n  \"title\": \"Google News RSS Feed Schema\",\n  \"description\": \"JSON Schema representing the structure of Google News RSS feed items.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"RSSFeed\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"channel\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"title\": {\n              \"type\": \"string\",\n              \"description\": \"The title of the RSS channel.\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The URL of the channel.\"\n            },\n            \"description\": {\n              \"type\": \"string\",\n              \"description\": \"Description of the channel.\"\n\
  \            },\n            \"language\": {\n              \"type\": \"string\",\n              \"description\": \"The language of the channel.\"\n            },\n            \"lastBuildDate\": {\n              \"type\": \"string\",\n              \"description\": \"The last build date of the feed.\"\n            },\n            \"items\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/NewsItem\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"NewsItem\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The headline of the news article.\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the news article.\"\n        },\n        \"pubDate\": {\n          \"type\": \"string\",\n          \"description\": \"Publication date\
  \ of the article.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A brief summary or snippet of the article.\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The news source name.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-news/refs/heads/main/json-schema/google-news.json
tags:
- Aggregation
- Google News
- Headlines
- Media
- News
- RSS
title: Google News RSS Feed Schema
---
