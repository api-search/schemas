---
description: A Slack conversation object representing a channel, direct message, multi-person direct message, or group conversation. This is the unified model returned by the conversations.* family of Web API methods, which consolidated the legacy channels.*, groups.*, im.*, and mpim.* endpoints. The type of conversation is identified by boolean flags (is_channel, is_group, is_im, is_mpim) and the is_private flag. Channels are uniquely identified by their id field, with public channels starting with C, private channels and multi-person DMs starting with G, and direct messages starting with D.
layout: schema
name: Slack Channel
properties_list:
- description: The unique identifier for this conversation. Public channels begin with C, private channels and multi-person DMs begin with G, and direct messages begin with D.
  name: id
  type: string
- description: 'The name of the channel without the leading # sign. Channel names can contain lowercase letters, numbers, hyphens, and underscores, with a maximum length of 80 characters. Not present for direct messa'
  name: name
  type: string
- description: A normalized, lowercase version of the channel name. Useful for case-insensitive comparisons and sorting.
  name: name_normalized
  type: string
- description: Whether this conversation is a public channel. Public channels are visible to all members of the workspace and can be joined by anyone.
  name: is_channel
  type: boolean
- description: Whether this conversation is a private channel. Private channels are invite-only and not visible in the channel browser.
  name: is_group
  type: boolean
- description: Whether this conversation is a direct message between two people.
  name: is_im
  type: boolean
- description: Whether this conversation is a multi-person direct message. MPIMs are group DMs between 3 or more people.
  name: is_mpim
  type: boolean
- description: Whether this conversation is private. True for private channels, DMs, and MPIMs. False for public channels.
  name: is_private
  type: boolean
- description: Whether the channel is archived. Archived channels are read-only and do not accept new messages. They can be unarchived by workspace admins.
  name: is_archived
  type: boolean
- description: 'Whether this is the workspace''s #general channel. Every workspace has exactly one general channel that all members are automatically added to.'
  name: is_general
  type: boolean
- description: Whether the channel is shared with another workspace using Slack Connect.
  name: is_shared
  type: boolean
- description: Whether the channel is shared with an external organization via Slack Connect. External shared channels allow cross-organization collaboration.
  name: is_ext_shared
  type: boolean
- description: Whether the channel is shared across the entire Enterprise Grid organization. Org-wide channels are available to all workspaces in the grid.
  name: is_org_shared
  type: boolean
- description: Whether there is a pending Slack Connect invitation for this channel that has not yet been accepted.
  name: is_pending_ext_shared
  type: boolean
- description: Whether the authenticated user or bot is a member of this conversation. Users must be members to read history or post messages in private channels.
  name: is_member
  type: boolean
- description: Whether the direct message or MPIM is currently open in the user's sidebar. Only relevant for DMs and MPIMs.
  name: is_open
  type: boolean
- description: Whether the channel is frozen. Frozen channels do not accept new messages.
  name: is_frozen
  type: boolean
- description: Whether the channel is read-only. In read-only channels, only admins and approved users can post.
  name: is_read_only
  type: boolean
- description: Whether the channel only allows threaded replies. Top-level posts are not permitted.
  name: is_thread_only
  type: boolean
- description: Whether threading is disabled in this channel.
  name: is_non_threadable
  type: boolean
- description: Unix timestamp (in seconds) of when the conversation was created.
  name: created
  type: integer
- description: The user ID of the member who created this channel. Not present for DMs.
  name: creator
  type: string
- description: Unix timestamp of the last update to the conversation metadata (not the last message).
  name: updated
  type: integer
- description: The number of times this shared channel has been unlinked from a partner workspace.
  name: unlinked
  type: integer
- description: The channel's topic. Topics appear below the channel name in the Slack client and help describe what the channel is currently being used for.
  name: topic
  type: object
- description: The channel's purpose. Purposes describe the intended use of the channel and help users decide whether to join.
  name: purpose
  type: object
- description: A list of all previous names this channel has had. Useful for tracking channel history and identifying channels that have been renamed.
  name: previous_names
  type: array
- description: The approximate number of members in the channel. Only included in responses when explicitly requested via the include_num_members parameter. May not be perfectly accurate for large channels.
  name: num_members
  type: integer
- description: The IETF language code for the channel's locale. Only included in responses when explicitly requested via the include_locale parameter.
  name: locale
  type: string
- description: For direct messages, the user ID of the other participant. Not present for channels, groups, or MPIMs.
  name: user
  type: string
- description: An array of team (workspace) IDs that share this channel. Present for shared and Slack Connect channels.
  name: shared_team_ids
  type: array
- description: An array of team IDs for pending shared channel invitations.
  name: pending_shared
  type: array
- description: An array of team IDs for pending Slack Connect invitations.
  name: pending_connected_team_ids
  type: array
- description: The parent conversation ID if this is a sub-conversation or thread-only channel. Null for top-level conversations.
  name: parent_conversation
  type:
  - string
  - 'null'
- description: The team (workspace) ID providing context for this conversation. Useful in Enterprise Grid environments where channels may be shared across workspaces.
  name: context_team_id
  type: string
- description: Additional channel properties including canvas and tab configurations.
  name: properties
  type: object
- description: The timestamp of the last message read by the authenticated user in this channel.
  name: last_read
  type: string
- description: The most recent message in the channel. Only included in some API responses.
  name: latest
  type: object
- description: The number of unread messages the authenticated user has in this channel.
  name: unread_count
  type: integer
- description: The number of unread messages to display (may differ from unread_count based on notification settings).
  name: unread_count_display
  type: integer
- description: A priority value used for sorting channels in the sidebar.
  name: priority
  type: number
provider_name: Slack
provider_slug: slack
schema_file: json-schema/slack-channel-schema.json
slug: slack-channel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.slack.dev/channel\",\n  \"title\": \"Slack Channel\",\n  \"description\": \"A Slack conversation object representing a channel, direct message, multi-person direct message, or group conversation. This is the unified model returned by the conversations.* family of Web API methods, which consolidated the legacy channels.*, groups.*, im.*, and mpim.* endpoints. The type of conversation is identified by boolean flags (is_channel, is_group, is_im, is_mpim) and the is_private flag. Channels are uniquely identified by their id field, with public channels starting with C, private channels and multi-person DMs starting with G, and direct messages starting with D.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"created\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for this conversation. Public channels\
  \ begin with C, private channels and multi-person DMs begin with G, and direct messages begin with D.\",\n      \"pattern\": \"^[CGDW][A-Z0-9]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the channel without the leading # sign. Channel names can contain lowercase letters, numbers, hyphens, and underscores, with a maximum length of 80 characters. Not present for direct messages.\",\n      \"maxLength\": 80,\n      \"pattern\": \"^[a-z0-9][a-z0-9_-]*$\"\n    },\n    \"name_normalized\": {\n      \"type\": \"string\",\n      \"description\": \"A normalized, lowercase version of the channel name. Useful for case-insensitive comparisons and sorting.\"\n    },\n    \"is_channel\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this conversation is a public channel. Public channels are visible to all members of the workspace and can be joined by anyone.\"\n    },\n    \"is_group\": {\n      \"type\": \"boolean\",\n      \"\
  description\": \"Whether this conversation is a private channel. Private channels are invite-only and not visible in the channel browser.\"\n    },\n    \"is_im\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this conversation is a direct message between two people.\"\n    },\n    \"is_mpim\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this conversation is a multi-person direct message. MPIMs are group DMs between 3 or more people.\"\n    },\n    \"is_private\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this conversation is private. True for private channels, DMs, and MPIMs. False for public channels.\"\n    },\n    \"is_archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is archived. Archived channels are read-only and do not accept new messages. They can be unarchived by workspace admins.\"\n    },\n    \"is_general\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ this is the workspace's #general channel. Every workspace has exactly one general channel that all members are automatically added to.\"\n    },\n    \"is_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is shared with another workspace using Slack Connect.\"\n    },\n    \"is_ext_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is shared with an external organization via Slack Connect. External shared channels allow cross-organization collaboration.\"\n    },\n    \"is_org_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is shared across the entire Enterprise Grid organization. Org-wide channels are available to all workspaces in the grid.\"\n    },\n    \"is_pending_ext_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether there is a pending Slack Connect invitation for this channel that has not yet been accepted.\"\n    },\n    \"is_member\": {\n\
  \      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated user or bot is a member of this conversation. Users must be members to read history or post messages in private channels.\"\n    },\n    \"is_open\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the direct message or MPIM is currently open in the user's sidebar. Only relevant for DMs and MPIMs.\"\n    },\n    \"is_frozen\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is frozen. Frozen channels do not accept new messages.\"\n    },\n    \"is_read_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel is read-only. In read-only channels, only admins and approved users can post.\"\n    },\n    \"is_thread_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the channel only allows threaded replies. Top-level posts are not permitted.\"\n    },\n    \"is_non_threadable\": {\n      \"type\": \"boolean\",\n\
  \      \"description\": \"Whether threading is disabled in this channel.\"\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp (in seconds) of when the conversation was created.\"\n    },\n    \"creator\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the member who created this channel. Not present for DMs.\",\n      \"pattern\": \"^[UW][A-Z0-9]+$\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the last update to the conversation metadata (not the last message).\"\n    },\n    \"unlinked\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of times this shared channel has been unlinked from a partner workspace.\"\n    },\n    \"topic\": {\n      \"type\": \"object\",\n      \"description\": \"The channel's topic. Topics appear below the channel name in the Slack client and help describe what the channel is currently being used for.\",\n  \
  \    \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The topic text. Supports mrkdwn formatting. Maximum 250 characters.\",\n          \"maxLength\": 250\n        },\n        \"creator\": {\n          \"type\": \"string\",\n          \"description\": \"The user ID of the person who last set the topic.\",\n          \"pattern\": \"^[UW][A-Z0-9]*$\"\n        },\n        \"last_set\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp of when the topic was last set. 0 if never set.\"\n        }\n      },\n      \"required\": [\n        \"value\",\n        \"creator\",\n        \"last_set\"\n      ]\n    },\n    \"purpose\": {\n      \"type\": \"object\",\n      \"description\": \"The channel's purpose. Purposes describe the intended use of the channel and help users decide whether to join.\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The\
  \ purpose text. Supports mrkdwn formatting. Maximum 250 characters.\",\n          \"maxLength\": 250\n        },\n        \"creator\": {\n          \"type\": \"string\",\n          \"description\": \"The user ID of the person who last set the purpose.\",\n          \"pattern\": \"^[UW][A-Z0-9]*$\"\n        },\n        \"last_set\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp of when the purpose was last set. 0 if never set.\"\n        }\n      },\n      \"required\": [\n        \"value\",\n        \"creator\",\n        \"last_set\"\n      ]\n    },\n    \"previous_names\": {\n      \"type\": \"array\",\n      \"description\": \"A list of all previous names this channel has had. Useful for tracking channel history and identifying channels that have been renamed.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"num_members\": {\n      \"type\": \"integer\",\n      \"description\": \"The approximate number of members in the\
  \ channel. Only included in responses when explicitly requested via the include_num_members parameter. May not be perfectly accurate for large channels.\",\n      \"minimum\": 0\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"The IETF language code for the channel's locale. Only included in responses when explicitly requested via the include_locale parameter.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"For direct messages, the user ID of the other participant. Not present for channels, groups, or MPIMs.\",\n      \"pattern\": \"^[UW][A-Z0-9]+$\"\n    },\n    \"shared_team_ids\": {\n      \"type\": \"array\",\n      \"description\": \"An array of team (workspace) IDs that share this channel. Present for shared and Slack Connect channels.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^T[A-Z0-9]+$\"\n      }\n    },\n    \"pending_shared\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"An array of team IDs for pending shared channel invitations.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pending_connected_team_ids\": {\n      \"type\": \"array\",\n      \"description\": \"An array of team IDs for pending Slack Connect invitations.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"parent_conversation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The parent conversation ID if this is a sub-conversation or thread-only channel. Null for top-level conversations.\"\n    },\n    \"context_team_id\": {\n      \"type\": \"string\",\n      \"description\": \"The team (workspace) ID providing context for this conversation. Useful in Enterprise Grid environments where channels may be shared across workspaces.\",\n      \"pattern\": \"^T[A-Z0-9]+$\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Additional channel properties including canvas and tab configurations.\"\
  ,\n      \"properties\": {\n        \"tabs\": {\n          \"type\": \"array\",\n          \"description\": \"An array of tab objects associated with the channel.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"label\": {\n                \"type\": \"string\"\n              },\n              \"type\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"canvas\": {\n          \"type\": \"object\",\n          \"description\": \"The channel canvas configuration.\",\n          \"properties\": {\n            \"file_id\": {\n              \"type\": \"string\"\n            },\n            \"is_empty\": {\n              \"type\": \"boolean\"\n            },\n            \"quip_thread_id\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"last_read\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of the last message read by the authenticated user in this channel.\",\n      \"pattern\": \"^[0-9]+\\\\.[0-9]+$\"\n    },\n    \"latest\": {\n      \"type\": \"object\",\n      \"description\": \"The most recent message in the channel. Only included in some API responses.\"\n    },\n    \"unread_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of unread messages the authenticated user has in this channel.\",\n      \"minimum\": 0\n    },\n    \"unread_count_display\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of unread messages to display (may differ from unread_count based on notification settings).\",\n      \"minimum\": 0\n    },\n    \"priority\": {\n      \"type\": \"number\",\n      \"description\": \"A priority value used for sorting channels in the sidebar.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slack/refs/heads/main/json-schema/slack-channel-schema.json
tags:
- Bots
- Chat
- Collaboration
- Messaging
- Productivity
- T1
- Team Communication
title: Slack Channel
---
