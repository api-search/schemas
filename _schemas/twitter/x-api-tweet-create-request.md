---
description: TweetCreateRequest schema from X API v2
layout: schema
name: TweetCreateRequest
properties_list:
- description: Card Uri Parameter. This is mutually exclusive from Quote Tweet Id, Poll, Media, and Direct Message Deep Link.
  name: card_uri
  type: string
- description: The unique identifier of this Community.
  name: community_id
  type: string
- description: Link to take the conversation from the public timeline to a private Direct Message.
  name: direct_message_deep_link
  type: string
- description: Options for editing an existing Post. When provided, this request will edit the specified Post instead of creating a new one.
  name: edit_options
  type: object
- description: Exclusive Tweet for super followers.
  name: for_super_followers_only
  type: boolean
- description: Place ID being attached to the Tweet for geo location.
  name: geo
  type: object
- description: Whether this Post contains AI-generated media. When true, the Post will be labeled accordingly.
  name: made_with_ai
  type: boolean
- description: Media information being attached to created Tweet. This is mutually exclusive from Quote Tweet Id, Poll, and Card URI.
  name: media
  type: object
- description: Nullcasted (promoted-only) Posts do not appear in the public timeline and are not served to followers.
  name: nullcast
  type: boolean
- description: Whether this Post is a paid partnership. When true, the Post will be labeled as a paid promotion.
  name: paid_partnership
  type: boolean
- description: Poll options for a Tweet with a poll. This is mutually exclusive from Media, Quote Tweet Id, and Card URI.
  name: poll
  type: object
- description: Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: quote_tweet_id
  type: string
- description: Tweet information of the Tweet being replied to.
  name: reply
  type: object
- description: Settings to indicate who can reply to the Tweet.
  name: reply_settings
  type: string
- description: Share community post with followers too.
  name: share_with_followers
  type: boolean
- description: The content of the Tweet.
  name: text
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-tweet-create-request-schema.json
slug: x-api-tweet-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-tweet-create-request-schema.json\",\n  \"title\": \"TweetCreateRequest\",\n  \"description\": \"TweetCreateRequest schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"card_uri\": {\n      \"type\": \"string\",\n      \"description\": \"Card Uri Parameter. This is mutually exclusive from Quote Tweet Id, Poll, Media, and Direct Message Deep Link.\"\n    },\n    \"community_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of this Community.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1146654567674912769\"\n    },\n    \"direct_message_deep_link\": {\n      \"type\": \"string\",\n      \"description\": \"Link to take the conversation from the public timeline to a private Direct Message.\"\n    },\n    \"edit_options\": {\n     \
  \ \"type\": \"object\",\n      \"description\": \"Options for editing an existing Post. When provided, this request will edit the specified Post instead of creating a new one.\",\n      \"required\": [\n        \"previous_post_id\"\n      ],\n      \"properties\": {\n        \"previous_post_id\": {\n          \"$ref\": \"#/components/schemas/TweetId\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"for_super_followers_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Exclusive Tweet for super followers.\",\n      \"default\": false\n    },\n    \"geo\": {\n      \"type\": \"object\",\n      \"description\": \"Place ID being attached to the Tweet for geo location.\",\n      \"properties\": {\n        \"place_id\": {\n          \"type\": \"string\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"made_with_ai\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this Post contains AI-generated media. When\
  \ true, the Post will be labeled accordingly.\"\n    },\n    \"media\": {\n      \"type\": \"object\",\n      \"description\": \"Media information being attached to created Tweet. This is mutually exclusive from Quote Tweet Id, Poll, and Card URI.\",\n      \"required\": [\n        \"media_ids\"\n      ],\n      \"properties\": {\n        \"media_ids\": {\n          \"type\": \"array\",\n          \"description\": \"A list of Media Ids to be attached to a created Tweet.\",\n          \"minItems\": 1,\n          \"maxItems\": 4,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/MediaId\"\n          }\n        },\n        \"tagged_user_ids\": {\n          \"type\": \"array\",\n          \"description\": \"A list of User Ids to be tagged in the media for created Tweet.\",\n          \"minItems\": 0,\n          \"maxItems\": 10,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/UserId\"\n          }\n        }\n      },\n      \"additionalProperties\"\
  : false\n    },\n    \"nullcast\": {\n      \"type\": \"boolean\",\n      \"description\": \"Nullcasted (promoted-only) Posts do not appear in the public timeline and are not served to followers.\",\n      \"default\": false\n    },\n    \"paid_partnership\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this Post is a paid partnership. When true, the Post will be labeled as a paid promotion.\"\n    },\n    \"poll\": {\n      \"type\": \"object\",\n      \"description\": \"Poll options for a Tweet with a poll. This is mutually exclusive from Media, Quote Tweet Id, and Card URI.\",\n      \"required\": [\n        \"options\",\n        \"duration_minutes\"\n      ],\n      \"properties\": {\n        \"duration_minutes\": {\n          \"type\": \"integer\",\n          \"description\": \"Duration of the poll in minutes.\",\n          \"minimum\": 5,\n          \"maximum\": 10080,\n          \"format\": \"int32\"\n        },\n        \"options\": {\n          \"type\": \"\
  array\",\n          \"minItems\": 2,\n          \"maxItems\": 4,\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"The text of a poll choice.\",\n            \"minLength\": 1,\n            \"maxLength\": 25\n          }\n        },\n        \"reply_settings\": {\n          \"type\": \"string\",\n          \"description\": \"Settings to indicate who can reply to the Tweet.\",\n          \"enum\": [\n            \"following\",\n            \"mentionedUsers\",\n            \"subscribers\",\n            \"verified\"\n          ]\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"quote_tweet_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1346889436626259968\"\n    },\n    \"reply\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Tweet information of the Tweet being replied to.\",\n      \"required\": [\n        \"in_reply_to_tweet_id\"\n      ],\n      \"properties\": {\n        \"auto_populate_reply_metadata\": {\n          \"type\": \"boolean\",\n          \"description\": \"If set to true, reply metadata will be automatically populated.\"\n        },\n        \"exclude_reply_user_ids\": {\n          \"type\": \"array\",\n          \"description\": \"A list of User Ids to be excluded from the reply Tweet.\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/UserId\"\n          }\n        },\n        \"in_reply_to_tweet_id\": {\n          \"$ref\": \"#/components/schemas/TweetId\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"reply_settings\": {\n      \"type\": \"string\",\n      \"description\": \"Settings to indicate who can reply to the Tweet.\",\n      \"enum\": [\n        \"following\",\n        \"mentionedUsers\",\n\
  \        \"subscribers\",\n        \"verified\"\n      ]\n    },\n    \"share_with_followers\": {\n      \"type\": \"boolean\",\n      \"description\": \"Share community post with followers too.\",\n      \"default\": false\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the Tweet.\",\n      \"example\": \"Learn how to use the user Tweet timeline and user mention timeline endpoints in the X API v2 to explore Tweet\\\\u2026 https:\\\\/\\\\/t.co\\\\/56a0vZUx7i\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-tweet-create-request-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: TweetCreateRequest
---
