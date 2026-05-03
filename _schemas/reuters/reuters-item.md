---
description: A content item from the Reuters Connect API representing a piece of editorial content such as a news story, image, video clip, or graphic. Items follow the IPTC NewsML-G2 standard and may be Simple News Items (SNI), News Event Packages (NEP), or Super News Event Packages (SNEP) for composite content.
layout: schema
name: Reuters Connect Content Item
properties_list:
- description: The unique identifier for the item, typically in tag URI format (e.g., tag:reuters.com,2025:newsml_L1N3KT0AB:1). Includes the version number as a suffix.
  name: id
  type: string
- description: A globally unique identifier for the item regardless of version. This identifier remains stable across revisions of the same content.
  name: guid
  type: string
- description: The version number of this item revision. Incremented each time the item is updated.
  name: version
  type: string
- description: The headline or title of the content item. For text stories, this is the story headline. For images and video, this is the caption title.
  name: headline
  type: string
- description: A short keyword slug summarizing the item topic, typically used for internal categorization and routing.
  name: slug
  type: string
- description: The date and time when the item was originally created, in ISO 8601 format.
  name: dateCreated
  type: string
- description: The date and time when the item was last modified, in ISO 8601 format.
  name: dateModified
  type: string
- description: The alias of the channel this item belongs to. Channels represent curated feeds of editorial content.
  name: channel
  type: string
- description: The media type classification of the content item.
  name: mediaType
  type: string
- description: The editorial urgency priority of the item, following the IPTC urgency scale where 1 is the most urgent and 9 is the least urgent.
  name: urgency
  type: integer
- description: The author or creator attribution for the item. May include the reporter name, photographer name, or agency credit.
  name: byline
  type: string
- description: The location and date line for the item, typically formatted as CITY, Month Day (e.g., NEW YORK, March 4).
  name: dateline
  type: string
- description: The ISO 639-1 language code of the content.
  name: language
  type: string
- description: The full text body of the content item. For text items, this contains the story body which may include XHTML markup. For media items, this may contain a caption or extended description.
  name: body
  type: string
- description: Subject classification codes assigned to the item, following the IPTC NewsCodes taxonomy for consistent categorization.
  name: subjects
  type: array
- description: Available renditions of the content. For images and video, this includes different sizes, resolutions, and formats available for download.
  name: renditions
  type: array
- description: Related items associated with this content, such as images accompanying a text story, video related to an event, or other cross-referenced editorial content.
  name: associations
  type: array
provider_name: Reuters
provider_slug: reuters
schema_file: json-schema/reuters-item-schema.json
slug: reuters-item
source_filename: reuters-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/reuters/json-schema/reuters-item-schema.json\",\n  \"title\": \"Reuters Connect Content Item\",\n  \"description\": \"A content item from the Reuters Connect API representing a piece of editorial content such as a news story, image, video clip, or graphic. Items follow the IPTC NewsML-G2 standard and may be Simple News Items (SNI), News Event Packages (NEP), or Super News Event Packages (SNEP) for composite content.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"headline\",\n    \"dateCreated\",\n    \"mediaType\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the item, typically in tag URI format (e.g., tag:reuters.com,2025:newsml_L1N3KT0AB:1). Includes the version number as a suffix.\",\n      \"examples\": [\n        \"tag:reuters.com,2025:newsml_L1N3KT0AB:1\"\n      ]\n\
  \    },\n    \"guid\": {\n      \"type\": \"string\",\n      \"description\": \"A globally unique identifier for the item regardless of version. This identifier remains stable across revisions of the same content.\",\n      \"examples\": [\n        \"tag:reuters.com,2025:newsml_L1N3KT0AB\"\n      ]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version number of this item revision. Incremented each time the item is updated.\",\n      \"examples\": [\n        \"1\",\n        \"2\"\n      ]\n    },\n    \"headline\": {\n      \"type\": \"string\",\n      \"description\": \"The headline or title of the content item. For text stories, this is the story headline. For images and video, this is the caption title.\",\n      \"maxLength\": 500\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"A short keyword slug summarizing the item topic, typically used for internal categorization and routing.\",\n      \"examples\": [\n  \
  \      \"USA-ELECTION\",\n        \"MARKETS-STOCKS\",\n        \"SOCCER-CHAMPIONS\"\n      ]\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the item was originally created, in ISO 8601 format.\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the item was last modified, in ISO 8601 format.\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"The alias of the channel this item belongs to. Channels represent curated feeds of editorial content.\"\n    },\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"The media type classification of the content item.\",\n      \"enum\": [\n        \"TEXT\",\n        \"PICTURE\",\n        \"VIDEO\",\n        \"GRAPHIC\",\n        \"COMPOSITE\"\n      ]\n    },\n    \"urgency\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"The editorial urgency priority of the item, following the IPTC urgency scale where 1 is the most urgent and 9 is the least urgent.\",\n      \"minimum\": 1,\n      \"maximum\": 9\n    },\n    \"byline\": {\n      \"type\": \"string\",\n      \"description\": \"The author or creator attribution for the item. May include the reporter name, photographer name, or agency credit.\"\n    },\n    \"dateline\": {\n      \"type\": \"string\",\n      \"description\": \"The location and date line for the item, typically formatted as CITY, Month Day (e.g., NEW YORK, March 4).\",\n      \"examples\": [\n        \"NEW YORK, March 4\",\n        \"LONDON, Feb 28\"\n      ]\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 639-1 language code of the content.\",\n      \"examples\": [\n        \"en\",\n        \"fr\",\n        \"de\",\n        \"es\"\n      ]\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The full text body of the content item. For text items, this contains the story body which may include XHTML markup. For media items, this may contain a caption or extended description.\"\n    },\n    \"subjects\": {\n      \"type\": \"array\",\n      \"description\": \"Subject classification codes assigned to the item, following the IPTC NewsCodes taxonomy for consistent categorization.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/subject\"\n      }\n    },\n    \"renditions\": {\n      \"type\": \"array\",\n      \"description\": \"Available renditions of the content. For images and video, this includes different sizes, resolutions, and formats available for download.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/rendition\"\n      }\n    },\n    \"associations\": {\n      \"type\": \"array\",\n      \"description\": \"Related items associated with this content, such as images accompanying a text story, video related to an event, or other cross-referenced editorial content.\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/association\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"subject\": {\n      \"type\": \"object\",\n      \"description\": \"A subject classification code from the IPTC NewsCodes taxonomy.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"The IPTC subject code identifier.\",\n          \"examples\": [\n            \"04000000\",\n            \"11000000\"\n          ]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable name of the subject category.\",\n          \"examples\": [\n            \"economy, business and finance\",\n            \"politics\"\n          ]\n        }\n      }\n    },\n    \"rendition\": {\n      \"type\": \"object\",\n      \"description\": \"A specific rendition or format of a media item available for download.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The name or label of the rendition indicating its purpose or size.\",\n          \"examples\": [\n            \"thumbnail\",\n            \"preview\",\n            \"baseImage\",\n            \"videoFile\"\n          ]\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL to download this rendition of the content.\"\n        },\n        \"mimetype\": {\n          \"type\": \"string\",\n          \"description\": \"The MIME type of the rendition file.\",\n          \"examples\": [\n            \"image/jpeg\",\n            \"video/mp4\",\n            \"application/pdf\"\n          ]\n        },\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"The width of the rendition in pixels (for images and video).\"\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"The height of the rendition in pixels\
  \ (for images and video).\"\n        },\n        \"sizeinbytes\": {\n          \"type\": \"integer\",\n          \"description\": \"The file size of the rendition in bytes.\"\n        }\n      }\n    },\n    \"association\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to an associated content item.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the associated item.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of association describing the relationship between items.\",\n          \"examples\": [\n            \"companion\",\n            \"related\",\n            \"seeAlso\"\n          ]\n        },\n        \"headline\": {\n          \"type\": \"string\",\n          \"description\": \"The headline of the associated item.\"\n        },\n        \"mediaType\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The media type of the associated item.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reuters/refs/heads/main/json-schema/reuters-item-schema.json
tags:
- Business
- Finance
- Journalism
- Media
- News
- Wire Service
title: Reuters Connect Content Item
---
