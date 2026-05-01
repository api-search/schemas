---
description: A media item resource from the Google Photos Library API representing a photo or video.
layout: schema
name: Google Photos Media Item
properties_list:
- description: Identifier for the media item.
  name: id
  type: string
- description: Description of the media item.
  name: description
  type: string
- description: A URL to the media item in Google Photos.
  name: productUrl
  type: string
- description: A URL to the bytes of the media item.
  name: baseUrl
  type: string
- description: MIME type of the media item.
  name: mimeType
  type: string
- description: Metadata related to the media item.
  name: mediaMetadata
  type: object
- description: Filename of the media item.
  name: filename
  type: string
provider_name: Google Photos Library
provider_slug: google-photos
schema_file: json-schema/photos.json
slug: photos
source_filename: photos.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-photos/refs/heads/main/json-schema/photos.json\",\n  \"title\": \"Google Photos Media Item\",\n  \"description\": \"A media item resource from the Google Photos Library API representing a photo or video.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the media item.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the media item.\"\n    },\n    \"productUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to the media item in Google Photos.\"\n    },\n    \"baseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to the bytes of the media item.\"\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"MIME type of the media item.\"\n    },\n    \"mediaMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata related to the media item.\",\n      \"properties\": {\n        \"creationTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Time when the media item was first created.\"\n        },\n        \"width\": {\n          \"type\": \"string\",\n          \"description\": \"Original width in pixels of the media item.\"\n        },\n        \"height\": {\n          \"type\": \"string\",\n          \"description\": \"Original height in pixels of the media item.\"\n        },\n        \"photo\": {\n          \"type\": \"object\",\n          \"description\": \"Metadata for a photo media type.\",\n          \"properties\": {\n            \"cameraMake\": {\n              \"type\": \"string\"\n            },\n            \"cameraModel\": {\n              \"type\": \"string\"\n            },\n\
  \            \"focalLength\": {\n              \"type\": \"number\"\n            },\n            \"apertureFNumber\": {\n              \"type\": \"number\"\n            },\n            \"isoEquivalent\": {\n              \"type\": \"integer\"\n            },\n            \"exposureTime\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"video\": {\n          \"type\": \"object\",\n          \"description\": \"Metadata for a video media type.\",\n          \"properties\": {\n            \"cameraMake\": {\n              \"type\": \"string\"\n            },\n            \"cameraModel\": {\n              \"type\": \"string\"\n            },\n            \"fps\": {\n              \"type\": \"number\"\n            },\n            \"status\": {\n              \"type\": \"string\",\n              \"enum\": [\"UNSPECIFIED\", \"PROCESSING\", \"READY\", \"FAILED\"]\n            }\n          }\n        }\n      }\n    },\n    \"filename\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Filename of the media item.\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-photos/refs/heads/main/json-schema/photos.json
tags:
- Albums
- Google
- Images
- Media
- Photos
- Sharing
- Storage
title: Google Photos Media Item
---
