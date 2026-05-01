---
description: A URL notification for the Google Indexing API to request crawling or removal.
layout: schema
name: Google Indexing URL Notification
properties_list:
- description: The URL to notify Google about.
  name: url
  type: string
- description: The type of notification.
  name: type
  type: string
- description: The time of the notification.
  name: notifyTime
  type: string
provider_name: Google Indexing
provider_slug: google-indexing
schema_file: json-schema/UrlNotification.json
slug: UrlNotification
source_filename: UrlNotification.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"UrlNotification.json\",\n  \"title\": \"Google Indexing URL Notification\",\n  \"description\": \"A URL notification for the Google Indexing API to request crawling or removal.\",\n  \"type\": \"object\",\n  \"required\": [\"url\", \"type\"],\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to notify Google about.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of notification.\",\n      \"enum\": [\n        \"URL_UPDATED\",\n        \"URL_DELETED\"\n      ]\n    },\n    \"notifyTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time of the notification.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-indexing/refs/heads/main/json-schema/UrlNotification.json
tags:
- Crawling
- Google
- Indexing
- Search
- SEO
- URLs
title: Google Indexing URL Notification
---
