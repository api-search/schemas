---
description: Represents media objects across Meta platforms including Facebook photos/videos and Instagram media (images, videos, carousels, reels, stories). Covers the Instagram Media node and Facebook Photo/Video nodes.
layout: schema
name: Meta Graph API Media
properties_list:
- description: The unique identifier for the media object.
  name: id
  type: string
- description: The type of media. IMAGE, VIDEO, and CAROUSEL_ALBUM are standard Instagram types; REEL and STORY are additional Instagram media types.
  name: media_type
  type: string
- description: The surface where the media is published (Instagram-specific).
  name: media_product_type
  type: string
- description: The URL of the media content. For videos this is the video URL; for images this is the image URL. Not returned for carousel albums.
  name: media_url
  type: string
- description: The URL of the media thumbnail. Only available for VIDEO media types.
  name: thumbnail_url
  type: string
- description: The permanent URL to the media on its platform (Instagram or Facebook).
  name: permalink
  type: string
- description: The shortcode identifier for the Instagram media (the code in the Instagram URL).
  name: shortcode
  type: string
- description: The caption/description text of the media.
  name: caption
  type: string
- description: The publication timestamp of the media in ISO 8601 format.
  name: timestamp
  type: string
- description: The username of the media owner (Instagram-specific).
  name: username
  type: string
- description: The owner of the media.
  name: owner
  type: object
- description: For Reels, whether the reel was also shared to the main feed.
  name: is_shared_to_feed
  type: boolean
- description: The number of likes on the media.
  name: like_count
  type: integer
- description: The number of comments on the media.
  name: comments_count
  type: integer
- description: Engagement insights for the media (Instagram Graph API).
  name: insights
  type: object
- description: Child media objects for CAROUSEL_ALBUM media types.
  name: children
  type: object
- description: The width of the media in pixels (Facebook photos/videos).
  name: width
  type: integer
- description: The height of the media in pixels (Facebook photos/videos).
  name: height
  type: integer
- description: The source URL for the media file (Facebook video source URL).
  name: source
  type: string
- description: Different size renditions of the image (Facebook Photo node).
  name: images
  type: array
- description: Different format renditions of the video (Facebook Video node).
  name: format
  type: array
- description: The album the photo belongs to (Facebook Photo node).
  name: album
  type: object
- description: The location tagged in the media.
  name: place
  type: object
- description: Users tagged in the media.
  name: tags
  type: object
- description: The time the media was created (Facebook Photo/Video nodes), in ISO 8601 format.
  name: created_time
  type: string
- description: The time the media was last updated, in ISO 8601 format.
  name: updated_time
  type: string
provider_name: Meta
provider_slug: meta
schema_file: json-schema/media.json
slug: media
source_filename: media.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://meta.com/schemas/graph-api/media.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Meta Graph API Media\",\n  \"description\": \"Represents media objects across Meta platforms including Facebook photos/videos and Instagram media (images, videos, carousels, reels, stories). Covers the Instagram Media node and Facebook Photo/Video nodes.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the media object.\"\n    },\n    \"media_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IMAGE\",\n        \"VIDEO\",\n        \"CAROUSEL_ALBUM\",\n        \"REEL\",\n        \"STORY\"\n      ],\n      \"description\": \"The type of media. IMAGE, VIDEO, and CAROUSEL_ALBUM are standard Instagram types; REEL and STORY are additional Instagram media types.\"\n    },\n    \"media_product_type\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AD\",\n        \"FEED\",\n        \"STORY\",\n        \"REELS\"\n      ],\n      \"description\": \"The surface where the media is published (Instagram-specific).\"\n    },\n    \"media_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the media content. For videos this is the video URL; for images this is the image URL. Not returned for carousel albums.\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the media thumbnail. Only available for VIDEO media types.\"\n    },\n    \"permalink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The permanent URL to the media on its platform (Instagram or Facebook).\"\n    },\n    \"shortcode\": {\n      \"type\": \"string\",\n      \"description\": \"The shortcode identifier for the Instagram media (the code in the\
  \ Instagram URL).\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"The caption/description text of the media.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The publication timestamp of the media in ISO 8601 format.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the media owner (Instagram-specific).\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"description\": \"The owner of the media.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The user/page ID of the media owner.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the media owner (Facebook).\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the media owner (Instagram).\"\
  \n        }\n      }\n    },\n    \"is_shared_to_feed\": {\n      \"type\": \"boolean\",\n      \"description\": \"For Reels, whether the reel was also shared to the main feed.\"\n    },\n    \"like_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of likes on the media.\"\n    },\n    \"comments_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of comments on the media.\"\n    },\n    \"insights\": {\n      \"type\": \"object\",\n      \"description\": \"Engagement insights for the media (Instagram Graph API).\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The metric name (e.g. impressions, reach, engagement, saved, video_views).\"\n              },\n              \"period\": {\n                \"type\": \"\
  string\",\n                \"description\": \"The aggregation period (e.g. lifetime).\"\n              },\n              \"values\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"value\": {\n                      \"type\": \"integer\"\n                    }\n                  }\n                }\n              },\n              \"title\": {\n                \"type\": \"string\"\n              },\n              \"description\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"children\": {\n      \"type\": \"object\",\n      \"description\": \"Child media objects for CAROUSEL_ALBUM media types.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n    \
  \            \"type\": \"string\"\n              },\n              \"media_type\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"IMAGE\",\n                  \"VIDEO\"\n                ]\n              },\n              \"media_url\": {\n                \"type\": \"string\",\n                \"format\": \"uri\"\n              },\n              \"timestamp\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"The width of the media in pixels (Facebook photos/videos).\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"The height of the media in pixels (Facebook photos/videos).\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The source URL for the media file (Facebook video\
  \ source URL).\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"description\": \"Different size renditions of the image (Facebook Photo node).\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"height\": {\n            \"type\": \"integer\"\n          },\n          \"width\": {\n            \"type\": \"integer\"\n          },\n          \"source\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      }\n    },\n    \"format\": {\n      \"type\": \"array\",\n      \"description\": \"Different format renditions of the video (Facebook Video node).\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"embed_html\": {\n            \"type\": \"string\"\n          },\n          \"filter\": {\n            \"type\": \"string\"\n          },\n          \"height\": {\n            \"type\": \"integer\"\n          },\n          \"width\": {\n          \
  \  \"type\": \"integer\"\n          },\n          \"picture\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      }\n    },\n    \"album\": {\n      \"type\": \"object\",\n      \"description\": \"The album the photo belongs to (Facebook Photo node).\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"place\": {\n      \"type\": \"object\",\n      \"description\": \"The location tagged in the media.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"location\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"latitude\": {\n              \"type\": \"number\"\n            },\n            \"longitude\": {\n              \"type\": \"number\"\n            },\n            \"\
  city\": {\n              \"type\": \"string\"\n            },\n            \"country\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Users tagged in the media.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"x\": {\n                \"type\": \"number\",\n                \"description\": \"X-coordinate of the tag as a percentage of the image width (0-100).\"\n              },\n              \"y\": {\n                \"type\": \"number\",\n                \"description\": \"Y-coordinate of the tag as a percentage of the image height (0-100).\"\n              }\n        \
  \    }\n          }\n        }\n      }\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the media was created (Facebook Photo/Video nodes), in ISO 8601 format.\"\n    },\n    \"updated_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the media was last updated, in ISO 8601 format.\"\n    }\n  },\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"id\": \"17895695668004550\",\n      \"media_type\": \"IMAGE\",\n      \"media_product_type\": \"FEED\",\n      \"media_url\": \"https://scontent.cdninstagram.com/v/example-image.jpg\",\n      \"permalink\": \"https://www.instagram.com/p/ABC123xyz/\",\n      \"shortcode\": \"ABC123xyz\",\n      \"caption\": \"Beautiful sunset at the beach #photography #nature\",\n      \"timestamp\": \"2025-07-10T18:30:00+0000\",\n      \"username\": \"examplephotographer\",\n      \"like_count\": 342,\n\
  \      \"comments_count\": 15,\n      \"owner\": {\n        \"id\": \"17841400123456789\",\n        \"username\": \"examplephotographer\"\n      }\n    },\n    {\n      \"id\": \"17895695668009999\",\n      \"media_type\": \"CAROUSEL_ALBUM\",\n      \"media_product_type\": \"FEED\",\n      \"permalink\": \"https://www.instagram.com/p/DEF456abc/\",\n      \"shortcode\": \"DEF456abc\",\n      \"caption\": \"Product launch highlights\",\n      \"timestamp\": \"2025-08-01T12:00:00+0000\",\n      \"username\": \"examplebrand\",\n      \"like_count\": 1580,\n      \"comments_count\": 92,\n      \"children\": {\n        \"data\": [\n          {\n            \"id\": \"17895695668010001\",\n            \"media_type\": \"IMAGE\",\n            \"media_url\": \"https://scontent.cdninstagram.com/v/carousel-1.jpg\"\n          },\n          {\n            \"id\": \"17895695668010002\",\n            \"media_type\": \"VIDEO\",\n            \"media_url\": \"https://scontent.cdninstagram.com/v/carousel-2.mp4\"\
  \n          }\n        ]\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/json-schema/media.json
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
title: Meta Graph API Media
---
