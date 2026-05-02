---
description: Represents a Facebook or Instagram post as returned by the Graph API Post node. Includes content, authorship, targeting, engagement metrics, and attached media.
layout: schema
name: Meta Graph API Post
properties_list:
- description: The unique identifier for the post, formatted as {page-id}_{post-id} for Page posts.
  name: id
  type: string
- description: The text content of the post.
  name: message
  type: string
- description: The auto-generated story text for system-generated posts (e.g. 'Jane updated her profile picture').
  name: story
  type: string
- description: The time the post was created, in ISO 8601 format.
  name: created_time
  type: string
- description: The time the post was last updated, in ISO 8601 format.
  name: updated_time
  type: string
- description: The user, Page, or entity that created the post.
  name: from
  type: object
- description: Profiles mentioned or targeted in the post.
  name: to
  type: object
- description: The permanent URL to the post on Facebook.
  name: permalink_url
  type: string
- description: URL to the full-size picture attached to the post.
  name: full_picture
  type: string
- description: URL to the thumbnail picture attached to the post.
  name: picture
  type: string
- description: URL to the icon representing the type of post.
  name: icon
  type: string
- description: The type of the post.
  name: type
  type: string
- description: A more descriptive classification of the post type.
  name: status_type
  type: string
- description: Whether the post is published (visible) or in draft/scheduled state.
  name: is_published
  type: boolean
- description: Whether the post has been hidden from the timeline.
  name: is_hidden
  type: boolean
- description: Whether the post has expired (for offer posts).
  name: is_expired
  type: boolean
- description: Whether the post is marked as popular based on engagement.
  name: is_popular
  type: boolean
- description: Whether the post is eligible to be promoted on Instagram.
  name: is_instagram_eligible
  type: boolean
- description: The privacy settings of the post.
  name: privacy
  type: object
- description: The location associated with the post.
  name: place
  type: object
- description: Share count for the post.
  name: shares
  type: object
- description: Summary of likes/reactions on the post.
  name: likes
  type: object
- description: Summary of comments on the post.
  name: comments
  type: object
- description: Media and link attachments on the post.
  name: attachments
  type: object
- description: Profiles tagged in the post message text.
  name: message_tags
  type: array
- description: The application that created the post.
  name: application
  type: object
- description: Unix timestamp for when a scheduled post will be published.
  name: scheduled_publish_time
  type: number
- description: The backdated time for the post, if it was backdated.
  name: backdated_time
  type: string
provider_name: Meta
provider_slug: meta
schema_file: json-schema/post.json
slug: post
source_filename: post.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://meta.com/schemas/graph-api/post.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Meta Graph API Post\",\n  \"description\": \"Represents a Facebook or Instagram post as returned by the Graph API Post node. Includes content, authorship, targeting, engagement metrics, and attached media.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the post, formatted as {page-id}_{post-id} for Page posts.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the post.\"\n    },\n    \"story\": {\n      \"type\": \"string\",\n      \"description\": \"The auto-generated story text for system-generated posts (e.g. 'Jane updated her profile picture').\"\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"The time the post was created, in ISO 8601 format.\"\n    },\n    \"updated_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the post was last updated, in ISO 8601 format.\"\n    },\n    \"from\": {\n      \"type\": \"object\",\n      \"description\": \"The user, Page, or entity that created the post.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"to\": {\n      \"type\": \"object\",\n      \"description\": \"Profiles mentioned or targeted in the post.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n     \
  \         }\n            }\n          }\n        }\n      }\n    },\n    \"permalink_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The permanent URL to the post on Facebook.\"\n    },\n    \"full_picture\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the full-size picture attached to the post.\"\n    },\n    \"picture\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the thumbnail picture attached to the post.\"\n    },\n    \"icon\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the icon representing the type of post.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"link\",\n        \"status\",\n        \"photo\",\n        \"video\",\n        \"offer\"\n      ],\n      \"description\": \"The type of the post.\"\n    },\n    \"status_type\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\n        \"mobile_status_update\",\n        \"created_note\",\n        \"added_photos\",\n        \"added_video\",\n        \"shared_story\",\n        \"created_group\",\n        \"created_event\",\n        \"wall_post\",\n        \"app_created_story\",\n        \"published_story\",\n        \"tagged_in_photo\",\n        \"approved_friend\"\n      ],\n      \"description\": \"A more descriptive classification of the post type.\"\n    },\n    \"is_published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is published (visible) or in draft/scheduled state.\"\n    },\n    \"is_hidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post has been hidden from the timeline.\"\n    },\n    \"is_expired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post has expired (for offer posts).\"\n    },\n    \"is_popular\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is marked\
  \ as popular based on engagement.\"\n    },\n    \"is_instagram_eligible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the post is eligible to be promoted on Instagram.\"\n    },\n    \"privacy\": {\n      \"type\": \"object\",\n      \"description\": \"The privacy settings of the post.\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"EVERYONE\",\n            \"ALL_FRIENDS\",\n            \"FRIENDS_OF_FRIENDS\",\n            \"SELF\",\n            \"CUSTOM\"\n          ],\n          \"description\": \"The privacy value of the post.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the privacy setting.\"\n        },\n        \"allow\": {\n          \"type\": \"string\",\n          \"description\": \"Comma-separated list of user IDs allowed to see the post.\"\n        },\n        \"deny\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Comma-separated list of user IDs denied from seeing the post.\"\n        }\n      }\n    },\n    \"place\": {\n      \"type\": \"object\",\n      \"description\": \"The location associated with the post.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"location\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"city\": {\n              \"type\": \"string\"\n            },\n            \"country\": {\n              \"type\": \"string\"\n            },\n            \"latitude\": {\n              \"type\": \"number\"\n            },\n            \"longitude\": {\n              \"type\": \"number\"\n            },\n            \"state\": {\n              \"type\": \"string\"\n            },\n            \"street\": {\n              \"type\": \"string\"\n            },\n            \"zip\": {\n      \
  \        \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"shares\": {\n      \"type\": \"object\",\n      \"description\": \"Share count for the post.\",\n      \"properties\": {\n        \"count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of times the post has been shared.\"\n        }\n      }\n    },\n    \"likes\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of likes/reactions on the post.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"summary\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"total_count\": {\n              \"type\"\
  : \"integer\"\n            },\n            \"can_like\": {\n              \"type\": \"boolean\"\n            },\n            \"has_liked\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"comments\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of comments on the post.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"message\": {\n                \"type\": \"string\"\n              },\n              \"from\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\"\n                  },\n                  \"name\": {\n                    \"type\": \"string\"\n                  }\n                }\n         \
  \     },\n              \"created_time\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\"\n              }\n            }\n          }\n        },\n        \"summary\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"total_count\": {\n              \"type\": \"integer\"\n            },\n            \"can_comment\": {\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"attachments\": {\n      \"type\": \"object\",\n      \"description\": \"Media and link attachments on the post.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"media_type\": {\n                \"type\": \"string\",\n                \"description\": \"The type of media (photo, video, link, album, etc.).\"\n              },\n              \"type\": {\n                \"type\"\
  : \"string\",\n                \"description\": \"The attachment type identifier.\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n                \"format\": \"uri\",\n                \"description\": \"URL of the attachment.\"\n              },\n              \"title\": {\n                \"type\": \"string\",\n                \"description\": \"Title of the attachment.\"\n              },\n              \"description\": {\n                \"type\": \"string\",\n                \"description\": \"Description of the attachment.\"\n              },\n              \"media\": {\n                \"type\": \"object\",\n                \"description\": \"The media object if the attachment contains media.\",\n                \"properties\": {\n                  \"image\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"height\": {\n                        \"type\": \"integer\"\n                \
  \      },\n                      \"src\": {\n                        \"type\": \"string\",\n                        \"format\": \"uri\"\n                      },\n                      \"width\": {\n                        \"type\": \"integer\"\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"message_tags\": {\n      \"type\": \"array\",\n      \"description\": \"Profiles tagged in the post message text.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"offset\": {\n            \"type\": \"integer\",\n            \"description\": \"Character offset into the message where the tag starts.\"\n          },\n          \"length\"\
  : {\n            \"type\": \"integer\",\n            \"description\": \"Length of the tagged text.\"\n          }\n        }\n      }\n    },\n    \"application\": {\n      \"type\": \"object\",\n      \"description\": \"The application that created the post.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"namespace\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"scheduled_publish_time\": {\n      \"type\": \"number\",\n      \"description\": \"Unix timestamp for when a scheduled post will be published.\"\n    },\n    \"backdated_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The backdated time for the post, if it was backdated.\"\n    }\n  },\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"id\": \"123456789012345_987654321098765\",\n      \"message\": \"Excited to announce\
  \ our new product launch!\",\n      \"created_time\": \"2025-06-15T14:30:00+0000\",\n      \"from\": {\n        \"id\": \"123456789012345\",\n        \"name\": \"Example Business Page\"\n      },\n      \"type\": \"photo\",\n      \"status_type\": \"added_photos\",\n      \"is_published\": true,\n      \"permalink_url\": \"https://www.facebook.com/examplebusiness/posts/987654321098765\",\n      \"full_picture\": \"https://scontent.xx.fbcdn.net/v/example-photo.jpg\",\n      \"shares\": {\n        \"count\": 42\n      },\n      \"likes\": {\n        \"summary\": {\n          \"total_count\": 1250,\n          \"can_like\": true,\n          \"has_liked\": false\n        }\n      },\n      \"comments\": {\n        \"summary\": {\n          \"total_count\": 89,\n          \"can_comment\": true\n        }\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/json-schema/post.json
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
title: Meta Graph API Post
---
