---
description: An Astronomy Picture of the Day entry from NASA's APOD service.
layout: schema
name: APOD Image
properties_list:
- description: The date of the APOD image (YYYY-MM-DD).
  name: date
  type: string
- description: Explanation of the image written by a professional astronomer.
  name: explanation
  type: string
- description: URL of the high-resolution image.
  name: hdurl
  type: string
- description: The type of media returned.
  name: media_type
  type: string
- description: The version of the APOD service.
  name: service_version
  type: string
- description: Title of the APOD image.
  name: title
  type: string
- description: URL of the image or video.
  name: url
  type: string
- description: Copyright holder of the image, if not public domain.
  name: copyright
  type: string
- description: URL of the video thumbnail when media_type is video.
  name: thumbnail_url
  type: string
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/apod-image.json
slug: apod-image
source_filename: apod-image.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/apod-image.json\",\n  \"title\": \"APOD Image\",\n  \"description\": \"An Astronomy Picture of the Day entry from NASA's APOD service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of the APOD image (YYYY-MM-DD).\"\n    },\n    \"explanation\": {\n      \"type\": \"string\",\n      \"description\": \"Explanation of the image written by a professional astronomer.\"\n    },\n    \"hdurl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the high-resolution image.\"\n    },\n    \"media_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"image\", \"video\"],\n      \"description\": \"The type of media returned.\"\n    },\n    \"service_version\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The version of the APOD service.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the APOD image.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the image or video.\"\n    },\n    \"copyright\": {\n      \"type\": \"string\",\n      \"description\": \"Copyright holder of the image, if not public domain.\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the video thumbnail when media_type is video.\"\n    }\n  },\n  \"required\": [\"date\", \"explanation\", \"media_type\", \"title\", \"url\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/apod-image.json
tags:
- Government
- Science
- Space
title: APOD Image
---
