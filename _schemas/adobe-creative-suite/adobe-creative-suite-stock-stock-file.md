---
description: Metadata for an Adobe Stock file
layout: schema
name: StockFile
properties_list:
- description: Unique Adobe Stock content identifier
  name: id
  type: integer
- description: Title of the stock file as provided by the contributor
  name: title
  type: string
- description: Display name of the file's creator/contributor
  name: creator_name
  type: string
- description: Unique identifier of the creator on Adobe Stock
  name: creator_id
  type: integer
- description: Country of origin of the creator
  name: country_name
  type: string
- description: Original width of the file in pixels
  name: width
  type: integer
- description: Original height of the file in pixels
  name: height
  type: integer
- description: Numeric identifier for the media type (1=photo, 2=illustration, 3=vector, 4=video, 6=3D, 7=template)
  name: media_type_id
  type: integer
- description: MIME type of the stock file
  name: content_type
  type: string
- description: List of keywords describing the file content
  name: keywords
  type: array
- description: URL of the watermarked comp image for preview purposes
  name: comp_url
  type: string
- description: URL of the thumbnail image
  name: thumbnail_url
  type: string
- description: Width of the thumbnail image in pixels
  name: thumbnail_width
  type: integer
- description: Height of the thumbnail image in pixels
  name: thumbnail_height
  type: integer
- description: Licensing status of the file for the authenticated user
  name: is_licensed
  type: string
- description: Vector file subtype (svg or zip) if applicable
  name: vector_type
  type: string
- description: ''
  name: category
  type: object
- description: Total number of results matching the search query (on first item only)
  name: nb_results
  type: integer
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-stock-file-schema.json
slug: adobe-creative-suite-stock-stock-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-stock-file-schema.json\",\n  \"title\": \"StockFile\",\n  \"description\": \"Metadata for an Adobe Stock file\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique Adobe Stock content identifier\",\n      \"example\": 123456789\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the stock file as provided by the contributor\",\n      \"example\": \"Beautiful mountain landscape at sunrise\"\n    },\n    \"creator_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the file's creator/contributor\",\n      \"example\": \"PhotoContributor123\"\n    },\n    \"creator_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier\
  \ of the creator on Adobe Stock\",\n      \"example\": 987654\n    },\n    \"country_name\": {\n      \"type\": \"string\",\n      \"description\": \"Country of origin of the creator\",\n      \"example\": \"United States\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Original width of the file in pixels\",\n      \"example\": 6000\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Original height of the file in pixels\",\n      \"example\": 4000\n    },\n    \"media_type_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the media type (1=photo, 2=illustration, 3=vector, 4=video, 6=3D, 7=template)\",\n      \"example\": 1\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the stock file\",\n      \"example\": \"image/jpeg\"\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"description\": \"List of keywords describing\
  \ the file content\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Keyword text\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"name\": \"mountain\"\n        },\n        {\n          \"name\": \"landscape\"\n        },\n        {\n          \"name\": \"sunrise\"\n        }\n      ]\n    },\n    \"comp_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the watermarked comp image for preview purposes\",\n      \"example\": \"https://t3.ftcdn.net/jpg/01/23/45/67/240_F_123456789_abc.jpg\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the thumbnail image\",\n      \"example\": \"https://t3.ftcdn.net/jpg/01/23/45/67/160_F_123456789_abc.jpg\"\n    },\n    \"thumbnail_width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width of the thumbnail image in pixels\"\
  ,\n      \"example\": 160\n    },\n    \"thumbnail_height\": {\n      \"type\": \"integer\",\n      \"description\": \"Height of the thumbnail image in pixels\",\n      \"example\": 107\n    },\n    \"is_licensed\": {\n      \"type\": \"string\",\n      \"description\": \"Licensing status of the file for the authenticated user\",\n      \"enum\": [\n        \"Standard\",\n        \"Extended\",\n        \"Video_HD\",\n        \"Video_4K\",\n        \"\"\n      ],\n      \"example\": \"\"\n    },\n    \"vector_type\": {\n      \"type\": \"string\",\n      \"description\": \"Vector file subtype (svg or zip) if applicable\",\n      \"enum\": [\n        \"svg\",\n        \"zip\",\n        \"\"\n      ],\n      \"example\": \"svg\"\n    },\n    \"category\": {\n      \"$ref\": \"#/components/schemas/Category\"\n    },\n    \"nb_results\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of results matching the search query (on first item only)\",\n      \"example\": 4521\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-stock-file-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: StockFile
---
