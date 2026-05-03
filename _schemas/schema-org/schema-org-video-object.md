---
description: A video file.
layout: schema
name: Schema.org VideoObject
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the video.
  name: name
  type: string
- description: A description of the video.
  name: description
  type: string
- description: URL of the video.
  name: url
  type: string
- description: Actual bytes of the media object.
  name: contentUrl
  type: string
- description: A URL pointing to a player for a specific video.
  name: embedUrl
  type: string
- description: A thumbnail image relevant to the video.
  name: thumbnailUrl
  type: object
- description: The duration of the video in ISO 8601 format.
  name: duration
  type: string
- description: Date when this video was uploaded.
  name: uploadDate
  type: string
- description: The caption for this video.
  name: caption
  type: string
- description: If this MediaObject is an AudioObject or VideoObject, the transcript of that object.
  name: transcript
  type: string
- description: The frame size of the video.
  name: videoFrameSize
  type: string
- description: The quality of the video.
  name: videoQuality
  type: string
- description: The width of the video in pixels.
  name: width
  type: integer
- description: The height of the video in pixels.
  name: height
  type: integer
- description: Media type expressed using a MIME format.
  name: encodingFormat
  type: string
- description: File size in bytes.
  name: contentSize
  type: string
- description: The bitrate of the media object.
  name: bitrate
  type: string
- description: Whether the video is family friendly.
  name: isFamilyFriendly
  type: boolean
- description: Indicates if use of the media requires a subscription.
  name: requiresSubscription
  type: boolean
- description: The regions where the video is allowed.
  name: regionsAllowed
  type: string
- description: The author of this video.
  name: author
  type: object
- description: The publisher of this video.
  name: publisher
  type: object
- description: Date of first publication.
  name: datePublished
  type: string
- description: The number of interactions for the video.
  name: interactionStatistic
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-video-object-schema.json
slug: schema-org-video-object
source_filename: schema-org-video-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/video-object.json\",\n  \"title\": \"Schema.org VideoObject\",\n  \"description\": \"A video file.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"VideoObject\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the video.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the video.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the video.\"\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"Actual bytes of the media object.\"\n    },\n    \"embedUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL pointing to a player for a specific video.\"\n    },\n    \"thumbnailUrl\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"A thumbnail image relevant to the video.\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"The duration of the video in ISO 8601 format.\"\n    },\n    \"uploadDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when this video was uploaded.\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"The caption for this video.\"\n    },\n    \"transcript\": {\n      \"type\": \"string\",\n      \"description\": \"If this MediaObject is an AudioObject\
  \ or VideoObject, the transcript of that object.\"\n    },\n    \"videoFrameSize\": {\n      \"type\": \"string\",\n      \"description\": \"The frame size of the video.\"\n    },\n    \"videoQuality\": {\n      \"type\": \"string\",\n      \"description\": \"The quality of the video.\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"The width of the video in pixels.\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"The height of the video in pixels.\"\n    },\n    \"encodingFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Media type expressed using a MIME format.\"\n    },\n    \"contentSize\": {\n      \"type\": \"string\",\n      \"description\": \"File size in bytes.\"\n    },\n    \"bitrate\": {\n      \"type\": \"string\",\n      \"description\": \"The bitrate of the media object.\"\n    },\n    \"isFamilyFriendly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the video is\
  \ family friendly.\"\n    },\n    \"requiresSubscription\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if use of the media requires a subscription.\"\n    },\n    \"regionsAllowed\": {\n      \"type\": \"string\",\n      \"description\": \"The regions where the video is allowed.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The author of this video.\"\n    },\n    \"publisher\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The publisher of this video.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"interactionStatistic\": {\n      \"type\": \"object\",\n    \
  \  \"description\": \"The number of interactions for the video.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"InteractionCounter\" },\n        \"interactionType\": { \"type\": \"string\" },\n        \"userInteractionCount\": { \"type\": \"integer\" }\n      }\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-video-object-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org VideoObject
---
