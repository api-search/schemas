---
description: The X User object.
layout: schema
name: User
properties_list:
- description: Metadata about a user's affiliation.
  name: affiliation
  type: object
- description: Returns detailed information about the relationship between two users.
  name: connection_status
  type: array
- description: Creation time of this User.
  name: created_at
  type: string
- description: The text of this User's profile description (also known as bio), if the User provided one.
  name: description
  type: string
- description: A list of metadata found in the User's profile description.
  name: entities
  type: object
- description: Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: id
  type: string
- description: The location specified in the User's profile, if the User provided one. As this is a freeform value, it may not indicate a valid location, but it may be fuzzily evaluated when performing searches with
  name: location
  type: string
- description: Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: most_recent_tweet_id
  type: string
- description: The friendly name of this User, as shown on their profile.
  name: name
  type: string
- description: Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: pinned_tweet_id
  type: string
- description: The URL to the profile banner for this User.
  name: profile_banner_url
  type: string
- description: The URL to the profile image for this User.
  name: profile_image_url
  type: string
- description: Indicates if this User has chosen to protect their Posts (in other words, if this User's Posts are private).
  name: protected
  type: boolean
- description: A list of metrics for this User.
  name: public_metrics
  type: object
- description: Indicates if you can send a DM to this User
  name: receives_your_dm
  type: boolean
- description: 'The X Blue subscription type of the user, eg: Basic, Premium, PremiumPlus or None.'
  name: subscription_type
  type: string
- description: The URL specified in the User's profile.
  name: url
  type: string
- description: The X handle (screen name) of this user.
  name: username
  type: string
- description: Indicate if this User is a verified X User.
  name: verified
  type: boolean
- description: 'The X Blue verified type of the user, eg: blue, government, business or none.'
  name: verified_type
  type: string
- description: Indicates withholding details for [withheld content](https://help.twitter.com/en/rules-and-policies/tweet-withheld-by-country).
  name: withheld
  type: object
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-user-schema.json
slug: x-api-user
source_filename: x-api-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"The X User object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"affiliation\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about a user's affiliation.\",\n      \"properties\": {\n        \"badge_url\": {\n          \"type\": \"string\",\n          \"description\": \"The badge URL corresponding to the affiliation.\",\n          \"format\": \"uri\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the affiliation.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"The URL, if available, to details about an affiliation.\",\n          \"format\": \"uri\"\n        },\n        \"user_id\": {\n  \
  \        \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/UserId\"\n          }\n        }\n      }\n    },\n    \"connection_status\": {\n      \"type\": \"array\",\n      \"description\": \"Returns detailed information about the relationship between two users.\",\n      \"minItems\": 0,\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Type of connection between users.\",\n        \"enum\": [\n          \"follow_request_received\",\n          \"follow_request_sent\",\n          \"blocking\",\n          \"followed_by\",\n          \"following\",\n          \"muting\"\n        ]\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Creation time of this User.\",\n      \"format\": \"date-time\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The text of this User's profile description (also known as bio), if the\
  \ User provided one.\"\n    },\n    \"entities\": {\n      \"type\": \"object\",\n      \"description\": \"A list of metadata found in the User's profile description.\",\n      \"properties\": {\n        \"description\": {\n          \"$ref\": \"#/components/schemas/FullTextEntities\"\n        },\n        \"url\": {\n          \"type\": \"object\",\n          \"description\": \"Expanded details for the URL specified in the User's profile, with start and end indices.\",\n          \"properties\": {\n            \"urls\": {\n              \"type\": \"array\",\n              \"minItems\": 1,\n              \"items\": {\n                \"$ref\": \"#/components/schemas/UrlEntity\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\"\
  : \"^[0-9]{1,19}$\",\n      \"example\": \"2244994945\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location specified in the User's profile, if the User provided one. As this is a freeform value, it may not indicate a valid location, but it may be fuzzily evaluated when performing searches with location queries.\"\n    },\n    \"most_recent_tweet_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1346889436626259968\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name of this User, as shown on their profile.\"\n    },\n    \"pinned_tweet_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this Tweet. This is returned as a string in order\
  \ to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1346889436626259968\"\n    },\n    \"profile_banner_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to the profile banner for this User.\",\n      \"format\": \"uri\"\n    },\n    \"profile_image_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to the profile image for this User.\",\n      \"format\": \"uri\"\n    },\n    \"protected\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if this User has chosen to protect their Posts (in other words, if this User's Posts are private).\"\n    },\n    \"public_metrics\": {\n      \"type\": \"object\",\n      \"description\": \"A list of metrics for this User.\",\n      \"required\": [\n        \"followers_count\",\n        \"following_count\",\n        \"tweet_count\",\n        \"listed_count\"\n      ],\n      \"properties\": {\n\
  \        \"followers_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of Users who are following this User.\"\n        },\n        \"following_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of Users this User is following.\"\n        },\n        \"like_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of likes created by this User.\"\n        },\n        \"listed_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of lists that include this User.\"\n        },\n        \"tweet_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of Posts (including Retweets) posted by this User.\"\n        }\n      }\n    },\n    \"receives_your_dm\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if you can send a DM to this User\"\n    },\n    \"subscription_type\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The X Blue subscription type of the user, eg: Basic, Premium, PremiumPlus or None.\",\n      \"enum\": [\n        \"Basic\",\n        \"Premium\",\n        \"PremiumPlus\",\n        \"None\"\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL specified in the User's profile.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The X handle (screen name) of this user.\",\n      \"pattern\": \"^[A-Za-z0-9_]{1,15}$\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicate if this User is a verified X User.\"\n    },\n    \"verified_type\": {\n      \"type\": \"string\",\n      \"description\": \"The X Blue verified type of the user, eg: blue, government, business or none.\",\n      \"enum\": [\n        \"blue\",\n        \"government\",\n        \"business\",\n        \"none\"\n      ]\n    },\n    \"withheld\": {\n      \"type\": \"object\",\n      \"description\": \"Indicates\
  \ withholding details for [withheld content](https://help.twitter.com/en/rules-and-policies/tweet-withheld-by-country).\",\n      \"required\": [\n        \"country_codes\"\n      ],\n      \"properties\": {\n        \"country_codes\": {\n          \"type\": \"array\",\n          \"description\": \"Provides a list of countries where this content is not available.\",\n          \"minItems\": 1,\n          \"uniqueItems\": true,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/CountryCode\"\n          }\n        },\n        \"scope\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates that the content being withheld is a `user`.\",\n          \"enum\": [\n            \"user\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"username\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-user-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: User
---
