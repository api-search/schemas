---
description: Schema for a single review returned from the Common Sense Media Reviews API v3.
layout: schema
name: Common Sense Media Review
properties_list:
- description: Unique identifier for the review.
  name: id
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: mediaType
  type: string
- description: ''
  name: langcode
  type: string
- description: Recommended minimum age.
  name: ageRating
  type: integer
- description: ''
  name: ageRatingGroup
  type: string
- description: Star rating out of five.
  name: stars
  type: integer
- description: ''
  name: oneLiner
  type: string
- description: ''
  name: anyGood
  type: string
- description: ''
  name: parentsNeedToKnow
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: talkingPoints
  type: array
- description: Per-criterion content ratings.
  name: contentGrid
  type: object
- description: Unix timestamp of last update.
  name: updated
  type: integer
provider_name: Common Sense Media
provider_slug: common-sense-media
schema_file: json-schema/common-sense-media-review-schema.json
slug: common-sense-media-review
source_filename: common-sense-media-review-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/common-sense-media/refs/heads/main/json-schema/common-sense-media-review-schema.json\",\n  \"title\": \"Common Sense Media Review\",\n  \"description\": \"Schema for a single review returned from the Common Sense Media Reviews API v3.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"mediaType\", \"title\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the review.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"enum\": [\"app\", \"book\", \"game\", \"movie\", \"podcast\", \"tv\", \"website\", \"youtube\"]\n    },\n    \"langcode\": {\n      \"type\": \"string\",\n      \"enum\": [\"en\", \"\
  es\"],\n      \"default\": \"en\"\n    },\n    \"ageRating\": {\n      \"type\": \"integer\",\n      \"minimum\": 2,\n      \"maximum\": 18,\n      \"description\": \"Recommended minimum age.\"\n    },\n    \"ageRatingGroup\": {\n      \"type\": \"string\",\n      \"enum\": [\"littleKids\", \"kids\", \"tweens\", \"teens\"]\n    },\n    \"stars\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 5,\n      \"description\": \"Star rating out of five.\"\n    },\n    \"oneLiner\": {\n      \"type\": \"string\"\n    },\n    \"anyGood\": {\n      \"type\": \"string\"\n    },\n    \"parentsNeedToKnow\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"talkingPoints\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"contentGrid\": {\n      \"type\": \"object\",\n      \"description\": \"Per-criterion content ratings.\",\n      \"additionalProperties\": {\n        \"type\": \"\
  object\",\n        \"properties\": {\n          \"rating\": { \"type\": \"integer\", \"minimum\": 0, \"maximum\": 5 },\n          \"label\": { \"type\": \"string\" },\n          \"text\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of last update.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/common-sense-media/refs/heads/main/json-schema/common-sense-media-review-schema.json
tags:
- Apps
- Books
- Media
- Movies
- Non-Profit
- Podcasts
- Ratings
- Reviews
- Television
- Video Games
- YouTube
title: Common Sense Media Review
---
