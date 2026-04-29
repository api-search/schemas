---
description: Schema for an Adobe Stock file record as returned by the Adobe Stock Search API. Represents a stock asset such as a photo, illustration, vector, video, or template including its metadata, creator information, dimensions, thumbnail URLs, and licensing status.
layout: schema
name: Adobe Stock File
properties_list:
- description: Unique Adobe Stock content identifier assigned to this file
  name: id
  type: integer
- description: Title of the stock file as provided by the contributor
  name: title
  type: string
- description: Display name of the contributor who created and uploaded this stock file
  name: creator_name
  type: string
- description: Unique identifier of the contributor on Adobe Stock
  name: creator_id
  type: integer
- description: Country of origin of the contributor as listed in their Adobe Stock profile
  name: country_name
  type: string
- description: Original width of the stock file in pixels (for images and video)
  name: width
  type: integer
- description: Original height of the stock file in pixels (for images and video)
  name: height
  type: integer
- description: 'Numeric identifier for the media type: 1=photo, 2=illustration, 3=vector, 4=video, 6=3D, 7=template'
  name: media_type_id
  type: integer
- description: MIME type of the stock file
  name: content_type
  type: string
- description: List of keyword objects describing the content and subject matter of the file
  name: keywords
  type: array
- description: URL of the watermarked comp image for preview and design mockup purposes. The comp is a lower-resolution, watermarked version of the full file.
  name: comp_url
  type: string
- description: URL of the small thumbnail image used in search result lists
  name: thumbnail_url
  type: string
- description: Width of the thumbnail image in pixels
  name: thumbnail_width
  type: integer
- description: Height of the thumbnail image in pixels
  name: thumbnail_height
  type: integer
- description: URL of a medium-size (500px) preview image
  name: thumbnail_500_url
  type: string
- description: URL of a larger (1000px) preview image
  name: thumbnail_1000_url
  type: string
- description: Licensing status of this file for the authenticated user. Empty string if not licensed.
  name: is_licensed
  type: string
- description: Vector file subtype for vector and illustration assets. Empty string for non-vector assets.
  name: vector_type
  type: string
- description: Primary category classification of this stock file
  name: category
  type: object
- description: 'Premium content level: 0=standard, 1=premium, 2=premium+'
  name: premium_level_id
  type: integer
- description: Whether this asset is editorial use only (not for commercial purposes)
  name: is_editorial
  type: boolean
- description: Whether this asset has model or property releases on file
  name: has_releases
  type: boolean
- description: Total number of results matching the search query. Only present on the first result in a search response.
  name: nb_results
  type: integer
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-stock-file-schema.json
slug: adobe-creative-suite-stock-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.adobe.com/ns/creative-suite/schemas/stock-file\",\n  \"title\": \"Adobe Stock File\",\n  \"description\": \"Schema for an Adobe Stock file record as returned by the Adobe Stock Search API. Represents a stock asset such as a photo, illustration, vector, video, or template including its metadata, creator information, dimensions, thumbnail URLs, and licensing status.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique Adobe Stock content identifier assigned to this file\",\n      \"examples\": [123456789]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the stock file as provided by the contributor\",\n      \"examples\": [\"Beautiful mountain landscape at sunrise with fog in the valley\"]\n    },\n    \"creator_name\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Display name of the contributor who created and uploaded this stock file\",\n      \"examples\": [\"PhotoContributor123\"]\n    },\n    \"creator_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the contributor on Adobe Stock\",\n      \"examples\": [987654]\n    },\n    \"country_name\": {\n      \"type\": \"string\",\n      \"description\": \"Country of origin of the contributor as listed in their Adobe Stock profile\",\n      \"examples\": [\"United States\", \"Germany\", \"Japan\"]\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Original width of the stock file in pixels (for images and video)\",\n      \"minimum\": 1,\n      \"examples\": [6000]\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Original height of the stock file in pixels (for images and video)\",\n      \"minimum\": 1,\n      \"examples\": [4000]\n    },\n    \"media_type_id\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Numeric identifier for the media type: 1=photo, 2=illustration, 3=vector, 4=video, 6=3D, 7=template\",\n      \"enum\": [1, 2, 3, 4, 6, 7],\n      \"examples\": [1]\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the stock file\",\n      \"examples\": [\"image/jpeg\", \"image/svg+xml\", \"video/mp4\", \"application/postscript\"]\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"description\": \"List of keyword objects describing the content and subject matter of the file\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single keyword associated with this stock file\",\n        \"required\": [\"name\"],\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Keyword text\",\n            \"examples\": [\"mountain\", \"landscape\", \"sunrise\", \"nature\"]\n         \
  \ }\n        },\n        \"additionalProperties\": false\n      },\n      \"examples\": [\n        [\n          {\"name\": \"mountain\"},\n          {\"name\": \"landscape\"},\n          {\"name\": \"sunrise\"},\n          {\"name\": \"nature\"},\n          {\"name\": \"fog\"}\n        ]\n      ]\n    },\n    \"comp_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the watermarked comp image for preview and design mockup purposes. The comp is a lower-resolution, watermarked version of the full file.\",\n      \"examples\": [\"https://t3.ftcdn.net/jpg/01/23/45/67/240_F_123456789_abc.jpg\"]\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the small thumbnail image used in search result lists\",\n      \"examples\": [\"https://t3.ftcdn.net/jpg/01/23/45/67/160_F_123456789_abc.jpg\"]\n    },\n    \"thumbnail_width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width of the thumbnail image in pixels\",\n      \"\
  minimum\": 1,\n      \"examples\": [160]\n    },\n    \"thumbnail_height\": {\n      \"type\": \"integer\",\n      \"description\": \"Height of the thumbnail image in pixels\",\n      \"minimum\": 1,\n      \"examples\": [107]\n    },\n    \"thumbnail_500_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of a medium-size (500px) preview image\",\n      \"examples\": [\"https://t3.ftcdn.net/jpg/01/23/45/67/500_F_123456789_abc.jpg\"]\n    },\n    \"thumbnail_1000_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of a larger (1000px) preview image\",\n      \"examples\": [\"https://t3.ftcdn.net/jpg/01/23/45/67/1000_F_123456789_abc.jpg\"]\n    },\n    \"is_licensed\": {\n      \"type\": \"string\",\n      \"description\": \"Licensing status of this file for the authenticated user. Empty string if not licensed.\",\n      \"enum\": [\"Standard\", \"Extended\", \"Video_HD\", \"Video_4K\", \"\"],\n      \"examples\": [\"Standard\", \"\"]\n    },\n    \"vector_type\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Vector file subtype for vector and illustration assets. Empty string for non-vector assets.\",\n      \"enum\": [\"svg\", \"zip\", \"\"],\n      \"examples\": [\"svg\", \"\"]\n    },\n    \"category\": {\n      \"type\": \"object\",\n      \"description\": \"Primary category classification of this stock file\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier of the category\",\n          \"examples\": [1043]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Localized display name of the category\",\n          \"examples\": [\"Nature\", \"Business\", \"Technology\", \"Animals\"]\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"premium_level_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Premium content level: 0=standard, 1=premium, 2=premium+\",\n      \"enum\": [0,\
  \ 1, 2],\n      \"examples\": [0]\n    },\n    \"is_editorial\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this asset is editorial use only (not for commercial purposes)\",\n      \"examples\": [false]\n    },\n    \"has_releases\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this asset has model or property releases on file\",\n      \"examples\": [true]\n    },\n    \"nb_results\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of results matching the search query. Only present on the first result in a search response.\",\n      \"minimum\": 0,\n      \"examples\": [4521]\n    }\n  },\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"id\": 123456789,\n      \"title\": \"Beautiful mountain landscape at sunrise with fog in the valley\",\n      \"creator_name\": \"PhotoContributor123\",\n      \"creator_id\": 987654,\n      \"country_name\": \"United States\",\n      \"width\": 6000,\n      \"height\"\
  : 4000,\n      \"media_type_id\": 1,\n      \"content_type\": \"image/jpeg\",\n      \"keywords\": [\n        {\"name\": \"mountain\"},\n        {\"name\": \"landscape\"},\n        {\"name\": \"sunrise\"},\n        {\"name\": \"nature\"},\n        {\"name\": \"fog\"}\n      ],\n      \"comp_url\": \"https://t3.ftcdn.net/jpg/01/23/45/67/240_F_123456789_abc.jpg\",\n      \"thumbnail_url\": \"https://t3.ftcdn.net/jpg/01/23/45/67/160_F_123456789_abc.jpg\",\n      \"thumbnail_width\": 160,\n      \"thumbnail_height\": 107,\n      \"is_licensed\": \"\",\n      \"vector_type\": \"\",\n      \"category\": {\n        \"id\": 1043,\n        \"name\": \"Nature\"\n      },\n      \"premium_level_id\": 0,\n      \"is_editorial\": false,\n      \"has_releases\": true,\n      \"nb_results\": 4521\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-stock-file-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: Adobe Stock File
---
