---
description: A Slack message object representing a single message in a conversation. Messages can contain plain text, Block Kit layouts, attachments, files, reactions, and metadata. Each message is uniquely identified by its channel and timestamp (ts) combination. Messages support threading via thread_ts, and can have subtypes indicating specialized message types such as bot_message, channel_join, file_share, etc.
layout: schema
name: Slack Message
properties_list:
- description: The object type. Always 'message' for message objects.
  name: type
  type: string
- description: 'An optional subtype indicating a specialized message type. Common subtypes include: bot_message, channel_join, channel_leave, channel_topic, channel_purpose, channel_name, channel_archive, channel_una'
  name: subtype
  type: string
- description: The channel ID where the message was posted. Channel IDs begin with C for public channels, G for private channels and multi-person DMs, and D for direct messages.
  name: channel
  type: string
- description: The user ID of the message author. User IDs begin with U or W.
  name: user
  type: string
- description: The text content of the message. Supports Slack mrkdwn formatting including *bold*, _italic_, ~strikethrough~, `code`, ```code blocks```, > blockquotes, and <URL|label> links. Also supports user menti
  name: text
  type: string
- description: The unique timestamp identifier for the message, which also serves as the message ID within its channel. Format is Unix epoch seconds with microsecond precision separated by a dot (e.g., '1503435956.0
  name: ts
  type: string
- description: The timestamp of the parent message when this message is a threaded reply. If present and equal to ts, this message is the parent of a thread. If present and different from ts, this message is a reply
  name: thread_ts
  type: string
- description: The total number of replies in the thread. Only present on the parent message of a thread.
  name: reply_count
  type: integer
- description: The number of unique users who have replied in the thread. Only present on the parent message.
  name: reply_users_count
  type: integer
- description: The timestamp of the most recent reply in the thread. Only present on the parent message.
  name: latest_reply
  type: string
- description: An array of user IDs for users who have replied in the thread. Only present on the parent message. Limited to the most recent 5 reply users by default.
  name: reply_users
  type: array
- description: Whether the thread is locked, preventing new replies.
  name: is_locked
  type: boolean
- description: Whether the authenticated user is subscribed to this thread.
  name: subscribed
  type: boolean
- description: An array of Block Kit layout blocks used for rich message formatting. Blocks can include sections, dividers, images, context, actions, header, input, and other interactive elements. See https://docs.s
  name: blocks
  type: array
- description: An array of secondary message attachments. While Block Kit is the preferred way to build rich messages, attachments are still supported for legacy compatibility and for displaying content below the bl
  name: attachments
  type: array
- description: An array of file objects attached to or shared in the message.
  name: files
  type: array
- description: An array of emoji reactions applied to this message. Only present when reactions exist.
  name: reactions
  type: array
- description: Metadata about when and by whom the message was last edited. Only present on edited messages.
  name: edited
  type: object
- description: The bot ID if this message was posted by a bot. Bot IDs begin with B.
  name: bot_id
  type: string
- description: Information about the bot that posted this message.
  name: bot_profile
  type: object
- description: The app ID if this message was posted by an app.
  name: app_id
  type: string
- description: Custom metadata attached to the message by an application. Metadata allows apps to attach structured data to messages for use in workflows and automations without affecting the visible message content
  name: metadata
  type: object
- description: A permanent URL pointing to this specific message within Slack.
  name: permalink
  type: string
- description: A unique identifier assigned by the client when the message was sent. Used for deduplication.
  name: client_msg_id
  type: string
- description: The team (workspace) ID where this message was posted.
  name: team
  type: string
- description: The user ID of the parent message author, if this is a threaded reply.
  name: parent_user_id
  type: string
- description: Whether the authenticated user has starred this message.
  name: is_starred
  type: boolean
- description: An array of channel IDs where this message is pinned.
  name: pinned_to
  type: array
- description: Whether the message is a file upload notification.
  name: upload
  type: boolean
- description: Whether the message should be displayed as if from a bot.
  name: display_as_bot
  type: boolean
provider_name: Slack
provider_slug: slack
schema_file: json-schema/slack-message-schema.json
slug: slack-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.slack.dev/message\",\n  \"title\": \"Slack Message\",\n  \"description\": \"A Slack message object representing a single message in a conversation. Messages can contain plain text, Block Kit layouts, attachments, files, reactions, and metadata. Each message is uniquely identified by its channel and timestamp (ts) combination. Messages support threading via thread_ts, and can have subtypes indicating specialized message types such as bot_message, channel_join, file_share, etc.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"type\",\n    \"ts\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"message\",\n      \"description\": \"The object type. Always 'message' for message objects.\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"An optional subtype indicating a specialized message type. Common\
  \ subtypes include: bot_message, channel_join, channel_leave, channel_topic, channel_purpose, channel_name, channel_archive, channel_unarchive, file_share, file_comment, me_message, thread_broadcast, tombstone, reminder_add, pinned_item, unpinned_item, and ekm_access_denied.\",\n      \"enum\": [\n        \"bot_message\",\n        \"channel_join\",\n        \"channel_leave\",\n        \"channel_topic\",\n        \"channel_purpose\",\n        \"channel_name\",\n        \"channel_archive\",\n        \"channel_unarchive\",\n        \"file_share\",\n        \"file_comment\",\n        \"me_message\",\n        \"thread_broadcast\",\n        \"tombstone\",\n        \"reminder_add\",\n        \"pinned_item\",\n        \"unpinned_item\",\n        \"ekm_access_denied\"\n      ]\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"The channel ID where the message was posted. Channel IDs begin with C for public channels, G for private channels and multi-person DMs, and\
  \ D for direct messages.\",\n      \"pattern\": \"^[CGDW][A-Z0-9]+$\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the message author. User IDs begin with U or W.\",\n      \"pattern\": \"^[UW][A-Z0-9]+$\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The text content of the message. Supports Slack mrkdwn formatting including *bold*, _italic_, ~strikethrough~, `code`, ```code blocks```, > blockquotes, and <URL|label> links. Also supports user mentions (<@U1234>), channel references (<#C1234>), and special commands (<!here>, <!channel>, <!everyone>).\"\n    },\n    \"ts\": {\n      \"type\": \"string\",\n      \"description\": \"The unique timestamp identifier for the message, which also serves as the message ID within its channel. Format is Unix epoch seconds with microsecond precision separated by a dot (e.g., '1503435956.000247'). The combination of channel and ts uniquely identifies any message in Slack.\"\
  ,\n      \"pattern\": \"^[0-9]+\\\\.[0-9]+$\"\n    },\n    \"thread_ts\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of the parent message when this message is a threaded reply. If present and equal to ts, this message is the parent of a thread. If present and different from ts, this message is a reply in the thread.\",\n      \"pattern\": \"^[0-9]+\\\\.[0-9]+$\"\n    },\n    \"reply_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of replies in the thread. Only present on the parent message of a thread.\",\n      \"minimum\": 0\n    },\n    \"reply_users_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of unique users who have replied in the thread. Only present on the parent message.\",\n      \"minimum\": 0\n    },\n    \"latest_reply\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of the most recent reply in the thread. Only present on the parent message.\",\n     \
  \ \"pattern\": \"^[0-9]+\\\\.[0-9]+$\"\n    },\n    \"reply_users\": {\n      \"type\": \"array\",\n      \"description\": \"An array of user IDs for users who have replied in the thread. Only present on the parent message. Limited to the most recent 5 reply users by default.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[UW][A-Z0-9]+$\"\n      }\n    },\n    \"is_locked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the thread is locked, preventing new replies.\"\n    },\n    \"subscribed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated user is subscribed to this thread.\"\n    },\n    \"blocks\": {\n      \"type\": \"array\",\n      \"description\": \"An array of Block Kit layout blocks used for rich message formatting. Blocks can include sections, dividers, images, context, actions, header, input, and other interactive elements. See https://docs.slack.dev/block-kit for the full Block Kit reference.\"\
  ,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"type\"\n        ],\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of block. Common types include section, divider, image, context, actions, header, input, file, rich_text, and video.\",\n            \"enum\": [\n              \"section\",\n              \"divider\",\n              \"image\",\n              \"context\",\n              \"actions\",\n              \"header\",\n              \"input\",\n              \"file\",\n              \"rich_text\",\n              \"video\",\n              \"call\"\n            ]\n          },\n          \"block_id\": {\n            \"type\": \"string\",\n            \"description\": \"A unique identifier for the block. If not provided, one will be generated. Maximum 255 characters.\",\n            \"maxLength\": 255\n          },\n          \"text\": {\n            \"type\": \"object\"\
  ,\n            \"description\": \"A text composition object. Used in section, header, and other blocks.\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"plain_text\",\n                  \"mrkdwn\"\n                ]\n              },\n              \"text\": {\n                \"type\": \"string\"\n              },\n              \"emoji\": {\n                \"type\": \"boolean\"\n              },\n              \"verbatim\": {\n                \"type\": \"boolean\"\n              }\n            }\n          },\n          \"elements\": {\n            \"type\": \"array\",\n            \"description\": \"An array of interactive elements or text objects within the block.\",\n            \"items\": {\n              \"type\": \"object\"\n            }\n          },\n          \"accessory\": {\n            \"type\": \"object\",\n            \"description\": \"An optional accessory element attached\
  \ to a section block.\"\n          },\n          \"fields\": {\n            \"type\": \"array\",\n            \"description\": \"An array of text objects for multi-column layouts in section blocks. Maximum of 10 items.\",\n            \"items\": {\n              \"type\": \"object\"\n            },\n            \"maxItems\": 10\n          }\n        }\n      }\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"An array of secondary message attachments. While Block Kit is the preferred way to build rich messages, attachments are still supported for legacy compatibility and for displaying content below the blocks.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"A unique identifier for this attachment within the message.\"\n          },\n          \"color\": {\n            \"type\": \"string\",\n            \"description\": \"A hex color\
  \ code used to color the left border of the attachment. Can be 'good' (green), 'warning' (yellow), 'danger' (red), or any hex code.\",\n            \"pattern\": \"^(#[0-9a-fA-F]{6}|good|warning|danger)$\"\n          },\n          \"fallback\": {\n            \"type\": \"string\",\n            \"description\": \"A plain text summary of the attachment used in notifications and clients that cannot render formatted text.\"\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"description\": \"The main body text of the attachment.\"\n          },\n          \"pretext\": {\n            \"type\": \"string\",\n            \"description\": \"Optional text that appears above the attachment block.\"\n          },\n          \"author_name\": {\n            \"type\": \"string\",\n            \"description\": \"Small text used to display the author's name.\"\n          },\n          \"author_link\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\
  ,\n            \"description\": \"A URL that will hyperlink the author_name.\"\n          },\n          \"author_icon\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"A URL that displays a small icon beside the author_name.\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"The title displayed in bold at the top of the attachment.\"\n          },\n          \"title_link\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"A URL that will hyperlink the title.\"\n          },\n          \"fields\": {\n            \"type\": \"array\",\n            \"description\": \"An array of field objects displayed in a table inside the attachment.\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"title\": {\n                  \"type\": \"string\",\n                  \"description\"\
  : \"The title of the field, shown as a bold heading.\"\n                },\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"The text value of the field.\"\n                },\n                \"short\": {\n                  \"type\": \"boolean\",\n                  \"description\": \"Whether the field is short enough to display side-by-side with other fields.\"\n                }\n              }\n            }\n          },\n          \"image_url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"A URL to an image to display inside the attachment.\"\n          },\n          \"thumb_url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"A URL to a thumbnail image to display to the right of the attachment.\"\n          },\n          \"footer\": {\n            \"type\": \"string\",\n            \"description\": \"Brief text\
  \ to contextualize and identify the attachment.\"\n          },\n          \"footer_icon\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"A URL for a small icon beside the footer text.\"\n          },\n          \"ts\": {\n            \"type\": \"integer\",\n            \"description\": \"A Unix timestamp to display alongside the footer.\"\n          },\n          \"mrkdwn_in\": {\n            \"type\": \"array\",\n            \"description\": \"An array of field names that should be formatted as mrkdwn.\",\n            \"items\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"text\",\n                \"pretext\",\n                \"fields\"\n              ]\n            }\n          },\n          \"actions\": {\n            \"type\": \"array\",\n            \"description\": \"An array of interactive message actions (legacy; prefer Block Kit).\",\n            \"items\": {\n              \"type\"\
  : \"object\"\n            }\n          },\n          \"callback_id\": {\n            \"type\": \"string\",\n            \"description\": \"An identifier for the set of actions in this attachment.\"\n          },\n          \"blocks\": {\n            \"type\": \"array\",\n            \"description\": \"Block Kit blocks within the attachment.\",\n            \"items\": {\n              \"type\": \"object\"\n            }\n          }\n        }\n      }\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"An array of file objects attached to or shared in the message.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique file identifier.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The filename.\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n       \
  \     \"description\": \"The title of the file.\"\n          },\n          \"mimetype\": {\n            \"type\": \"string\",\n            \"description\": \"The MIME type of the file.\"\n          },\n          \"filetype\": {\n            \"type\": \"string\",\n            \"description\": \"The Slack file type identifier.\"\n          },\n          \"size\": {\n            \"type\": \"integer\",\n            \"description\": \"File size in bytes.\"\n          },\n          \"url_private\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"Authenticated URL to access the file.\"\n          },\n          \"permalink\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"Permalink URL for the file.\"\n          },\n          \"mode\": {\n            \"type\": \"string\",\n            \"description\": \"The file mode (hosted, external, snippet, post).\",\n            \"enum\": [\n   \
  \           \"hosted\",\n              \"external\",\n              \"snippet\",\n              \"post\",\n              \"space\",\n              \"quip\"\n            ]\n          }\n        }\n      }\n    },\n    \"reactions\": {\n      \"type\": \"array\",\n      \"description\": \"An array of emoji reactions applied to this message. Only present when reactions exist.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"name\",\n          \"count\",\n          \"users\"\n        ],\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The emoji name without surrounding colons (e.g., 'thumbsup', 'heart', 'eyes').\"\n          },\n          \"count\": {\n            \"type\": \"integer\",\n            \"description\": \"The number of users who have applied this reaction.\",\n            \"minimum\": 1\n          },\n          \"users\": {\n            \"type\": \"array\",\n        \
  \    \"description\": \"An array of user IDs who applied this reaction.\",\n            \"items\": {\n              \"type\": \"string\",\n              \"pattern\": \"^[UW][A-Z0-9]+$\"\n            }\n          }\n        }\n      }\n    },\n    \"edited\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about when and by whom the message was last edited. Only present on edited messages.\",\n      \"properties\": {\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"The user ID of the person who edited the message.\",\n          \"pattern\": \"^[UW][A-Z0-9]+$\"\n        },\n        \"ts\": {\n          \"type\": \"string\",\n          \"description\": \"The timestamp of the edit.\",\n          \"pattern\": \"^[0-9]+\\\\.[0-9]+$\"\n        }\n      },\n      \"required\": [\n        \"user\",\n        \"ts\"\n      ]\n    },\n    \"bot_id\": {\n      \"type\": \"string\",\n      \"description\": \"The bot ID if this message was posted by\
  \ a bot. Bot IDs begin with B.\",\n      \"pattern\": \"^B[A-Z0-9]+$\"\n    },\n    \"bot_profile\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the bot that posted this message.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"deleted\": {\n          \"type\": \"boolean\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"updated\": {\n          \"type\": \"integer\"\n        },\n        \"app_id\": {\n          \"type\": \"string\"\n        },\n        \"icons\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"image_36\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"image_48\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"image_72\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n        \
  \    }\n          }\n        },\n        \"team_id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"The app ID if this message was posted by an app.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata attached to the message by an application. Metadata allows apps to attach structured data to messages for use in workflows and automations without affecting the visible message content.\",\n      \"properties\": {\n        \"event_type\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable identifier for the metadata event type.\"\n        },\n        \"event_payload\": {\n          \"type\": \"object\",\n          \"description\": \"A free-form JSON object containing the metadata payload.\"\n        }\n      },\n      \"required\": [\n        \"event_type\",\n        \"event_payload\"\n      ]\n    },\n    \"permalink\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A permanent URL pointing to this specific message within Slack.\"\n    },\n    \"client_msg_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier assigned by the client when the message was sent. Used for deduplication.\",\n      \"format\": \"uuid\"\n    },\n    \"team\": {\n      \"type\": \"string\",\n      \"description\": \"The team (workspace) ID where this message was posted.\",\n      \"pattern\": \"^T[A-Z0-9]+$\"\n    },\n    \"parent_user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the parent message author, if this is a threaded reply.\",\n      \"pattern\": \"^[UW][A-Z0-9]+$\"\n    },\n    \"is_starred\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated user has starred this message.\"\n    },\n    \"pinned_to\": {\n      \"type\": \"array\",\n      \"description\": \"An array of channel IDs\
  \ where this message is pinned.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^[CG][A-Z0-9]+$\"\n      }\n    },\n    \"upload\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the message is a file upload notification.\"\n    },\n    \"display_as_bot\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the message should be displayed as if from a bot.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/json-schema/slack-message-schema.json
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
title: Slack Message
---
