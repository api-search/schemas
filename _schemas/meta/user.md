---
description: Represents a Facebook or Instagram user account as returned by the Graph API User node. Covers identity, demographics, profile details, and engagement metrics.
layout: schema
name: Meta Graph API User
properties_list:
- description: The unique numeric identifier for the user, returned as a string by the Graph API.
  name: id
  type: string
- description: The full name of the user.
  name: name
  type: string
- description: The first name of the user.
  name: first_name
  type: string
- description: The last name of the user.
  name: last_name
  type: string
- description: The middle name of the user.
  name: middle_name
  type: string
- description: The user's name formatted to correctly handle Chinese, Japanese, or Korean ordering.
  name: name_format
  type: string
- description: Shortened, informal name for the user.
  name: short_name
  type: string
- description: The primary email address listed in the user's profile. Requires the email permission.
  name: email
  type: string
- description: The user's birthday in MM/DD/YYYY format. Requires the user_birthday permission.
  name: birthday
  type: string
- description: The gender selected by the user. This is a free-form string; common values are 'male', 'female', and 'non-binary'.
  name: gender
  type: string
- description: A link to the user's Facebook profile.
  name: link
  type: string
- description: The user's profile picture.
  name: picture
  type: object
- description: The user's locale as a language-country code string, e.g. en_US.
  name: locale
  type: string
- description: The user's timezone offset from UTC, expressed as a number (e.g. -5).
  name: timezone
  type: number
- description: The user's current location as entered on their profile.
  name: location
  type: object
- description: The user's hometown as entered on their profile.
  name: hometown
  type: object
- description: The age range of the user as a min/max bracket.
  name: age_range
  type: object
- description: Languages the user has added to their profile.
  name: languages
  type: array
- description: Whether the user has the application installed.
  name: installed
  type: boolean
- description: Whether the user account is a guest/limited account.
  name: is_guest_user
  type: boolean
- description: What the user is interested in meeting for (e.g. networking, dating).
  name: meeting_for
  type: array
- description: The user's favorite quotes.
  name: quotes
  type: string
- description: The user's significant other.
  name: significant_other
  type: object
- description: The last time the user's profile was updated, in ISO 8601 format.
  name: updated_time
  type: string
- description: The user's friends list (summary only by default).
  name: friends
  type: object
- description: The linked Instagram Business or Creator account, if any.
  name: instagram_business_account
  type: object
provider_name: Meta
provider_slug: meta
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://meta.com/schemas/graph-api/user.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Meta Graph API User\",\n  \"description\": \"Represents a Facebook or Instagram user account as returned by the Graph API User node. Covers identity, demographics, profile details, and engagement metrics.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique numeric identifier for the user, returned as a string by the Graph API.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the user.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the user.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the user.\"\n    },\n    \"middle_name\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The middle name of the user.\"\n    },\n    \"name_format\": {\n      \"type\": \"string\",\n      \"description\": \"The user's name formatted to correctly handle Chinese, Japanese, or Korean ordering.\"\n    },\n    \"short_name\": {\n      \"type\": \"string\",\n      \"description\": \"Shortened, informal name for the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The primary email address listed in the user's profile. Requires the email permission.\"\n    },\n    \"birthday\": {\n      \"type\": \"string\",\n      \"description\": \"The user's birthday in MM/DD/YYYY format. Requires the user_birthday permission.\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"description\": \"The gender selected by the user. This is a free-form string; common values are 'male', 'female', and 'non-binary'.\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"uri\",\n      \"description\": \"A link to the user's Facebook profile.\"\n    },\n    \"picture\": {\n      \"type\": \"object\",\n      \"description\": \"The user's profile picture.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"height\": {\n              \"type\": \"integer\",\n              \"description\": \"The height of the picture in pixels.\"\n            },\n            \"is_silhouette\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the profile picture is the default silhouette.\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL of the profile picture.\"\n            },\n            \"width\": {\n              \"type\": \"integer\",\n              \"description\": \"The width of the picture in pixels.\"\n            }\n          }\n       \
  \ }\n      }\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"The user's locale as a language-country code string, e.g. en_US.\"\n    },\n    \"timezone\": {\n      \"type\": \"number\",\n      \"description\": \"The user's timezone offset from UTC, expressed as a number (e.g. -5).\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"The user's current location as entered on their profile.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Graph API ID of the location Page.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the location.\"\n        }\n      }\n    },\n    \"hometown\": {\n      \"type\": \"object\",\n      \"description\": \"The user's hometown as entered on their profile.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The\
  \ Graph API ID of the hometown Page.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the hometown.\"\n        }\n      }\n    },\n    \"age_range\": {\n      \"type\": \"object\",\n      \"description\": \"The age range of the user as a min/max bracket.\",\n      \"properties\": {\n        \"min\": {\n          \"type\": \"integer\",\n          \"description\": \"The lower bound of the age range.\"\n        },\n        \"max\": {\n          \"type\": \"integer\",\n          \"description\": \"The upper bound of the age range.\"\n        }\n      }\n    },\n    \"languages\": {\n      \"type\": \"array\",\n      \"description\": \"Languages the user has added to their profile.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n   \
  \ \"installed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has the application installed.\"\n    },\n    \"is_guest_user\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is a guest/limited account.\"\n    },\n    \"meeting_for\": {\n      \"type\": \"array\",\n      \"description\": \"What the user is interested in meeting for (e.g. networking, dating).\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"quotes\": {\n      \"type\": \"string\",\n      \"description\": \"The user's favorite quotes.\"\n    },\n    \"significant_other\": {\n      \"type\": \"object\",\n      \"description\": \"The user's significant other.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"updated_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The last time the user's profile was updated, in ISO 8601 format.\"\n    },\n    \"friends\": {\n      \"type\": \"object\",\n      \"description\": \"The user's friends list (summary only by default).\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"summary\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"total_count\": {\n              \"type\": \"integer\",\n              \"description\": \"Total number of friends.\"\n            }\n          }\n        }\n      }\n    },\n    \"instagram_business_account\": {\n      \"type\": \"object\",\n      \"description\": \"The linked Instagram Business or Creator account, if\
  \ any.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Instagram account ID.\"\n        }\n      }\n    }\n  },\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"id\": \"10158012345678901\",\n      \"name\": \"Jane Developer\",\n      \"first_name\": \"Jane\",\n      \"last_name\": \"Developer\",\n      \"email\": \"jane@example.com\",\n      \"picture\": {\n        \"data\": {\n          \"height\": 200,\n          \"is_silhouette\": false,\n          \"url\": \"https://platform-lookaside.fbsbx.com/platform/profilepic/?asid=10158012345678901&height=200&width=200\",\n          \"width\": 200\n        }\n      },\n      \"locale\": \"en_US\",\n      \"timezone\": -5\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/json-schema/user.json
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
title: Meta Graph API User
---
