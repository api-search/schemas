---
description: An individual review of an app on Google Play, containing the user comment and optional developer reply.
layout: schema
name: Review
properties_list:
- description: Unique identifier for the review.
  name: reviewId
  type: string
- description: The name of the user who wrote the review.
  name: authorName
  type: string
- description: A list of comments for this review. Contains the user comment and optionally the developer reply.
  name: comments
  type: array
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-review-schema.json
slug: google-play-developer-review
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Review\",\n  \"type\": \"object\",\n  \"description\": \"An individual review of an app on Google Play, containing the user comment and optional developer reply.\",\n  \"properties\": {\n    \"reviewId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the review.\"\n    },\n    \"authorName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user who wrote the review.\"\n    },\n    \"comments\": {\n      \"type\": \"array\",\n      \"description\": \"A list of comments for this review. Contains the user comment and optionally the developer reply.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-review-schema.json
tags:
- AI
- Android
- Automotive
- Google
- Machine Learning
- Mobile Development
- SDK
- TV
- Wearables
title: Review
---
