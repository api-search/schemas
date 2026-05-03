---
description: A media object, such as an image, video, audio, or text object embedded in a web page or a downloadable dataset.
layout: schema
name: Schema.org MediaObject
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the media object.
  name: name
  type: string
- description: A description of the media object.
  name: description
  type: string
- description: URL of the media object.
  name: url
  type: string
- description: Actual bytes of the media object.
  name: contentUrl
  type: string
- description: A URL pointing to a player for the media.
  name: embedUrl
  type: string
- description: Media type expressed using a MIME format.
  name: encodingFormat
  type: string
- description: File size in bytes.
  name: contentSize
  type: string
- description: The bitrate of the media object.
  name: bitrate
  type: string
- description: The duration of the item in ISO 8601 format.
  name: duration
  type: string
- description: The width of the media.
  name: width
  type: object
- description: The height of the media.
  name: height
  type: object
- description: Player type required.
  name: playerType
  type: string
- description: The production company or studio performing the work.
  name: productionCompany
  type: object
- description: Date when this media object was uploaded.
  name: uploadDate
  type: string
- description: Indicates if use of the media requires a subscription.
  name: requiresSubscription
  type: boolean
- description: The regions where the media is allowed.
  name: regionsAllowed
  type: string
- description: A NewsArticle associated with the media object.
  name: associatedArticle
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-media-object-schema.json
slug: schema-org-media-object
source_filename: schema-org-media-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/media-object.json\",\n  \"title\": \"Schema.org MediaObject\",\n  \"description\": \"A media object, such as an image, video, audio, or text object embedded in a web page or a downloadable dataset.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"MediaObject\", \"AudioObject\", \"DataDownload\", \"ImageObject\", \"MusicVideoObject\", \"VideoObject\", \"3DModel\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the media object.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the media object.\"\n    },\n    \"url\": {\n   \
  \   \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the media object.\"\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Actual bytes of the media object.\"\n    },\n    \"embedUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL pointing to a player for the media.\"\n    },\n    \"encodingFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Media type expressed using a MIME format.\"\n    },\n    \"contentSize\": {\n      \"type\": \"string\",\n      \"description\": \"File size in bytes.\"\n    },\n    \"bitrate\": {\n      \"type\": \"string\",\n      \"description\": \"The bitrate of the media object.\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"The duration of the item in ISO 8601 format.\"\n    },\n    \"width\": {\n      \"oneOf\": [\n        { \"type\": \"integer\" },\n        { \"\
  type\": \"object\", \"properties\": { \"@type\": { \"const\": \"QuantitativeValue\" }, \"value\": { \"type\": \"integer\" }, \"unitCode\": { \"type\": \"string\" } } }\n      ],\n      \"description\": \"The width of the media.\"\n    },\n    \"height\": {\n      \"oneOf\": [\n        { \"type\": \"integer\" },\n        { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"QuantitativeValue\" }, \"value\": { \"type\": \"integer\" }, \"unitCode\": { \"type\": \"string\" } } }\n      ],\n      \"description\": \"The height of the media.\"\n    },\n    \"playerType\": {\n      \"type\": \"string\",\n      \"description\": \"Player type required.\"\n    },\n    \"productionCompany\": {\n      \"$ref\": \"schema-org-organization-schema.json\",\n      \"description\": \"The production company or studio performing the work.\"\n    },\n    \"uploadDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when this media object was uploaded.\"\
  \n    },\n    \"requiresSubscription\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if use of the media requires a subscription.\"\n    },\n    \"regionsAllowed\": {\n      \"type\": \"string\",\n      \"description\": \"The regions where the media is allowed.\"\n    },\n    \"associatedArticle\": {\n      \"$ref\": \"schema-org-article-schema.json\",\n      \"description\": \"A NewsArticle associated with the media object.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-media-object-schema.json
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
title: Schema.org MediaObject
---
