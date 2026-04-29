---
description: Tweet schema from X API v2
layout: schema
name: Tweet
properties_list:
- description: Specifies the type of attachments (if any) present in this Tweet.
  name: attachments
  type: object
- description: Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: author_id
  type: string
- description: The unique identifier of this Community.
  name: community_id
  type: string
- description: ''
  name: context_annotations
  type: array
- description: Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: conversation_id
  type: string
- description: Creation time of the Tweet.
  name: created_at
  type: string
- description: Represent a boundary range (start and end zero-based indices) for the portion of text that is displayed for a post. `start` must be smaller than `end`. The start index is inclusive, the end index is e
  name: display_text_range
  type: array
- description: ''
  name: edit_controls
  type: object
- description: A list of Tweet Ids in this Tweet chain.
  name: edit_history_tweet_ids
  type: array
- description: ''
  name: entities
  type: object
- description: The location tagged on the Tweet, if the user provided one.
  name: geo
  type: object
- description: Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: id
  type: string
- description: Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: in_reply_to_user_id
  type: string
- description: Language of the Tweet, if detected by X. Returned as a BCP47 language tag.
  name: lang
  type: string
- description: Nonpublic engagement metrics for the Tweet at the time of the request.
  name: non_public_metrics
  type: object
- description: The full-content of the Tweet, including text beyond 280 characters.
  name: note_tweet
  type: object
- description: Organic nonpublic engagement metrics for the Tweet at the time of the request.
  name: organic_metrics
  type: object
- description: Indicates if this Tweet contains URLs marked as sensitive, for example content suitable for mature audiences.
  name: possibly_sensitive
  type: boolean
- description: Promoted nonpublic engagement metrics for the Tweet at the time of the request.
  name: promoted_metrics
  type: object
- description: Engagement metrics for the Tweet at the time of the request.
  name: public_metrics
  type: object
- description: A list of Posts this Tweet refers to. For example, if the parent Tweet is a Retweet, a Quoted Tweet or a Reply, it will include the related Tweet referenced to by its parent.
  name: referenced_tweets
  type: array
- description: Shows who can reply a Tweet. Fields returned are everyone, mentioned_users, subscribers, verified and following.
  name: reply_settings
  type: string
- description: The scopes for this tweet
  name: scopes
  type: object
- description: This is deprecated.
  name: source
  type: string
- description: ''
  name: suggested_source_links
  type: array
- description: Suggested source links and the number of requests that included each link.
  name: suggested_source_links_with_counts
  type: object
- description: The content of the Tweet.
  name: text
  type: string
- description: The X handle (screen name) of this user.
  name: username
  type: string
- description: Indicates withholding details for [withheld content](https://help.twitter.com/en/rules-and-policies/tweet-withheld-by-country).
  name: withheld
  type: object
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-tweet-schema.json
slug: x-api-tweet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-tweet-schema.json\",\n  \"title\": \"Tweet\",\n  \"description\": \"Tweet schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attachments\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies the type of attachments (if any) present in this Tweet.\",\n      \"properties\": {\n        \"media_keys\": {\n          \"type\": \"array\",\n          \"description\": \"A list of Media Keys for each one of the media attachments (if media are attached).\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/MediaKey\"\n          }\n        },\n        \"media_source_tweet_id\": {\n          \"type\": \"array\",\n          \"description\": \"A list of Posts the media on this Tweet was originally posted in. For example, if the media\
  \ on a tweet is re-used in another Tweet, this refers to the original, source Tweet..\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/TweetId\"\n          }\n        },\n        \"poll_ids\": {\n          \"type\": \"array\",\n          \"description\": \"A list of poll IDs (if polls are attached).\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/PollId\"\n          }\n        }\n      }\n    },\n    \"author_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"2244994945\"\n    },\n    \"community_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of this Community.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\"\
  : \"1146654567674912769\"\n    },\n    \"context_annotations\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ContextAnnotation\"\n      }\n    },\n    \"conversation_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1346889436626259968\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Creation time of the Tweet.\",\n      \"format\": \"date-time\",\n      \"example\": \"2021-01-06T18:40:40.000Z\"\n    },\n    \"display_text_range\": {\n      \"type\": \"array\",\n      \"description\": \"Represent a boundary range (start and end zero-based indices) for the portion of text that is displayed for a post. `start` must be smaller than `end`. The start index\
  \ is inclusive, the end index is exclusive.\",\n      \"minItems\": 2,\n      \"maxItems\": 2,\n      \"items\": {\n        \"type\": \"integer\",\n        \"minimum\": 0\n      }\n    },\n    \"edit_controls\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"is_edit_eligible\",\n        \"editable_until\",\n        \"edits_remaining\"\n      ],\n      \"properties\": {\n        \"editable_until\": {\n          \"type\": \"string\",\n          \"description\": \"Time when Tweet is no longer editable.\",\n          \"format\": \"date-time\",\n          \"example\": \"2021-01-06T18:40:40.000Z\"\n        },\n        \"edits_remaining\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet can be edited.\"\n        },\n        \"is_edit_eligible\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates if this Tweet is eligible to be edited.\",\n          \"example\": false\n        }\n      }\n    },\n    \"edit_history_tweet_ids\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"A list of Tweet Ids in this Tweet chain.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TweetId\"\n      }\n    },\n    \"entities\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"annotations\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"description\": \"Annotation for entities based on the Tweet text.\",\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/EntityIndicesInclusiveInclusive\"\n              },\n              {\n                \"type\": \"object\",\n                \"description\": \"Represents the data for the annotation.\",\n                \"properties\": {\n                  \"normalized_text\": {\n                    \"type\": \"string\",\n                    \"description\": \"Text used to determine annotation.\",\n                    \"example\": \"\
  Barack Obama\"\n                  },\n                  \"probability\": {\n                    \"type\": \"number\",\n                    \"description\": \"Confidence factor for annotation type.\",\n                    \"minimum\": 0,\n                    \"maximum\": 1,\n                    \"format\": \"double\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"description\": \"Annotation type.\",\n                    \"example\": \"Person\"\n                  }\n                }\n              }\n            ]\n          }\n        },\n        \"cashtags\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/CashtagEntity\"\n          }\n        },\n        \"hashtags\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/HashtagEntity\"\n          }\n  \
  \      },\n        \"mentions\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/MentionEntity\"\n          }\n        },\n        \"urls\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/UrlEntity\"\n          }\n        }\n      }\n    },\n    \"geo\": {\n      \"type\": \"object\",\n      \"description\": \"The location tagged on the Tweet, if the user provided one.\",\n      \"properties\": {\n        \"coordinates\": {\n          \"$ref\": \"#/components/schemas/Point\"\n        },\n        \"place_id\": {\n          \"$ref\": \"#/components/schemas/PlaceId\"\n        }\n      }\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this Tweet. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n   \
  \   \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1346889436626259968\"\n    },\n    \"in_reply_to_user_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"2244994945\"\n    },\n    \"lang\": {\n      \"type\": \"string\",\n      \"description\": \"Language of the Tweet, if detected by X. Returned as a BCP47 language tag.\",\n      \"example\": \"en\"\n    },\n    \"non_public_metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Nonpublic engagement metrics for the Tweet at the time of the request.\",\n      \"properties\": {\n        \"impression_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been viewed.\",\n          \"format\": \"int32\"\n        }\n      }\n    },\n    \"note_tweet\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"The full-content of the Tweet, including text beyond 280 characters.\",\n      \"properties\": {\n        \"entities\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"cashtags\": {\n              \"type\": \"array\",\n              \"minItems\": 1,\n              \"items\": {\n                \"$ref\": \"#/components/schemas/CashtagEntity\"\n              }\n            },\n            \"hashtags\": {\n              \"type\": \"array\",\n              \"minItems\": 1,\n              \"items\": {\n                \"$ref\": \"#/components/schemas/HashtagEntity\"\n              }\n            },\n            \"mentions\": {\n              \"type\": \"array\",\n              \"minItems\": 1,\n              \"items\": {\n                \"$ref\": \"#/components/schemas/MentionEntity\"\n              }\n            },\n            \"urls\": {\n              \"type\": \"array\",\n              \"minItems\"\
  : 1,\n              \"items\": {\n                \"$ref\": \"#/components/schemas/UrlEntity\"\n              }\n            }\n          }\n        },\n        \"text\": {\n          \"$ref\": \"#/components/schemas/NoteTweetText\"\n        }\n      }\n    },\n    \"organic_metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Organic nonpublic engagement metrics for the Tweet at the time of the request.\",\n      \"required\": [\n        \"impression_count\",\n        \"retweet_count\",\n        \"reply_count\",\n        \"like_count\"\n      ],\n      \"properties\": {\n        \"impression_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been viewed.\"\n        },\n        \"like_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been liked.\"\n        },\n        \"reply_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times\
  \ this Tweet has been replied to.\"\n        },\n        \"retweet_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been Retweeted.\"\n        }\n      }\n    },\n    \"possibly_sensitive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if this Tweet contains URLs marked as sensitive, for example content suitable for mature audiences.\",\n      \"example\": false\n    },\n    \"promoted_metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Promoted nonpublic engagement metrics for the Tweet at the time of the request.\",\n      \"properties\": {\n        \"impression_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been viewed.\",\n          \"format\": \"int32\"\n        },\n        \"like_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been liked.\",\n          \"format\": \"int32\"\
  \n        },\n        \"reply_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been replied to.\",\n          \"format\": \"int32\"\n        },\n        \"retweet_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been Retweeted.\",\n          \"format\": \"int32\"\n        }\n      }\n    },\n    \"public_metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Engagement metrics for the Tweet at the time of the request.\",\n      \"required\": [\n        \"retweet_count\",\n        \"reply_count\",\n        \"like_count\",\n        \"impression_count\",\n        \"bookmark_count\"\n      ],\n      \"properties\": {\n        \"bookmark_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been bookmarked.\",\n          \"format\": \"int32\"\n        },\n        \"impression_count\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"Number of times this Tweet has been viewed.\",\n          \"format\": \"int32\"\n        },\n        \"like_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been liked.\"\n        },\n        \"quote_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been quoted.\"\n        },\n        \"reply_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been replied to.\"\n        },\n        \"retweet_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this Tweet has been Retweeted.\"\n        }\n      }\n    },\n    \"referenced_tweets\": {\n      \"type\": \"array\",\n      \"description\": \"A list of Posts this Tweet refers to. For example, if the parent Tweet is a Retweet, a Quoted Tweet or a Reply, it will include the related Tweet referenced to by its parent.\"\
  ,\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"type\",\n          \"id\"\n        ],\n        \"properties\": {\n          \"id\": {\n            \"$ref\": \"#/components/schemas/TweetId\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"retweeted\",\n              \"quoted\",\n              \"replied_to\"\n            ]\n          }\n        }\n      }\n    },\n    \"reply_settings\": {\n      \"type\": \"string\",\n      \"description\": \"Shows who can reply a Tweet. Fields returned are everyone, mentioned_users, subscribers, verified and following.\",\n      \"pattern\": \"^[A-Za-z]{1,12}$\",\n      \"enum\": [\n        \"everyone\",\n        \"mentionedUsers\",\n        \"following\",\n        \"other\",\n        \"subscribers\",\n        \"verified\"\n      ]\n    },\n    \"scopes\": {\n      \"type\": \"object\",\n      \"description\": \"The scopes\
  \ for this tweet\",\n      \"properties\": {\n        \"followers\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates if this Tweet is viewable by followers without the Tweet ID\",\n          \"example\": false\n        }\n      }\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"This is deprecated.\"\n    },\n    \"suggested_source_links\": {\n      \"type\": \"array\",\n      \"minItems\": 0,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UrlEntity\"\n      }\n    },\n    \"suggested_source_links_with_counts\": {\n      \"type\": \"object\",\n      \"description\": \"Suggested source links and the number of requests that included each link.\",\n      \"properties\": {\n        \"count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of note requests that included the source link.\"\n        },\n        \"url\": {\n          \"$ref\": \"#/components/schemas/UrlEntity\"\n        }\n   \
  \   }\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The content of the Tweet.\",\n      \"example\": \"Learn how to use the user Tweet timeline and user mention timeline endpoints in the X API v2 to explore Tweet\\\\u2026 https:\\\\/\\\\/t.co\\\\/56a0vZUx7i\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The X handle (screen name) of this user.\",\n      \"pattern\": \"^[A-Za-z0-9_]{1,15}$\"\n    },\n    \"withheld\": {\n      \"type\": \"object\",\n      \"description\": \"Indicates withholding details for [withheld content](https://help.twitter.com/en/rules-and-policies/tweet-withheld-by-country).\",\n      \"required\": [\n        \"copyright\",\n        \"country_codes\"\n      ],\n      \"properties\": {\n        \"copyright\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates if the content is being withheld for on the basis of copyright infringement.\"\n        },\n        \"country_codes\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"Provides a list of countries where this content is not available.\",\n          \"minItems\": 1,\n          \"uniqueItems\": true,\n          \"items\": {\n            \"$ref\": \"#/components/schemas/CountryCode\"\n          }\n        },\n        \"scope\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether the content being withheld is the `tweet` or a `user`.\",\n          \"enum\": [\n            \"tweet\",\n            \"user\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-tweet-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Tweet
---
