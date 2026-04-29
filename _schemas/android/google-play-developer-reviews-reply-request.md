---
description: Request body for replying to a review.
layout: schema
name: ReviewsReplyRequest
properties_list:
- description: The text of the reply. The reply will replace any existing reply. Maximum length is 350 characters.
  name: replyText
  type: string
provider_name: Android
provider_slug: android
schema_file: json-schema/google-play-developer-reviews-reply-request-schema.json
slug: google-play-developer-reviews-reply-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReviewsReplyRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for replying to a review.\",\n  \"properties\": {\n    \"replyText\": {\n      \"type\": \"string\",\n      \"description\": \"The text of the reply. The reply will replace any existing reply. Maximum length is 350 characters.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/android/refs/heads/main/json-schema/google-play-developer-reviews-reply-request-schema.json
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
title: ReviewsReplyRequest
---
