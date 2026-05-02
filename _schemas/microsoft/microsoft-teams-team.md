---
description: Represents a team in Microsoft Teams. A team is a collection of channels and members with shared settings, permissions, and tools for collaboration.
layout: schema
name: Microsoft Teams Team
properties_list:
- description: Unique identifier for the team (GUID)
  name: id
  type: string
- description: The name of the team
  name: displayName
  type: string
- description: An optional description for the team
  name: description
  type:
  - string
  - 'null'
- description: A unique ID for the team that has been used in some internal contexts
  name: internalId
  type:
  - string
  - 'null'
- description: An optional label describing the sensitivity of the team
  name: classification
  type:
  - string
  - 'null'
- description: Indicates whether the team is intended for a particular use case
  name: specialization
  type:
  - string
  - 'null'
- description: The visibility of the group and team
  name: visibility
  type:
  - string
  - 'null'
- description: A hyperlink to the team in the Microsoft Teams client
  name: webUrl
  type:
  - string
  - 'null'
- description: Whether this team is in read-only mode
  name: isArchived
  type:
  - boolean
  - 'null'
- description: If set to true, the team is currently in the owner-only team membership state
  name: isMembershipLimitedToOwners
  type:
  - boolean
  - 'null'
- description: Timestamp at which the team was created
  name: createdDateTime
  type:
  - string
  - 'null'
- description: ''
  name: memberSettings
  type: object
- description: ''
  name: guestSettings
  type: object
- description: ''
  name: messagingSettings
  type: object
- description: ''
  name: funSettings
  type: object
- description: ''
  name: discoverySettings
  type: object
provider_name: Microsoft
provider_slug: microsoft
schema_file: json-schema/microsoft-teams-team-schema.json
slug: microsoft-teams-team
source_filename: microsoft-teams-team-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/graph/schemas/microsoft/team.json\",\n  \"title\": \"Microsoft Teams Team\",\n  \"description\": \"Represents a team in Microsoft Teams. A team is a collection of channels and members with shared settings, permissions, and tools for collaboration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the team (GUID)\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the team\",\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional description for the team\",\n      \"maxLength\": 1024\n    },\n    \"internalId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A unique ID for the team that has been\
  \ used in some internal contexts\",\n      \"readOnly\": true\n    },\n    \"classification\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An optional label describing the sensitivity of the team\"\n    },\n    \"specialization\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"none\", \"educationStandard\", \"educationClass\", \"educationProfessionalLearningCommunity\", \"educationStaff\", \"unknownFutureValue\"],\n      \"description\": \"Indicates whether the team is intended for a particular use case\"\n    },\n    \"visibility\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"private\", \"public\"],\n      \"description\": \"The visibility of the group and team\"\n    },\n    \"webUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"A hyperlink to the team in the Microsoft Teams client\",\n      \"readOnly\": true\n    },\n    \"isArchived\": {\n      \"type\": [\"\
  boolean\", \"null\"],\n      \"description\": \"Whether this team is in read-only mode\"\n    },\n    \"isMembershipLimitedToOwners\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"If set to true, the team is currently in the owner-only team membership state\"\n    },\n    \"createdDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp at which the team was created\",\n      \"readOnly\": true\n    },\n    \"memberSettings\": {\n      \"$ref\": \"#/$defs/TeamMemberSettings\"\n    },\n    \"guestSettings\": {\n      \"$ref\": \"#/$defs/TeamGuestSettings\"\n    },\n    \"messagingSettings\": {\n      \"$ref\": \"#/$defs/TeamMessagingSettings\"\n    },\n    \"funSettings\": {\n      \"$ref\": \"#/$defs/TeamFunSettings\"\n    },\n    \"discoverySettings\": {\n      \"$ref\": \"#/$defs/TeamDiscoverySettings\"\n    }\n  },\n  \"$defs\": {\n    \"TeamMemberSettings\": {\n      \"type\": [\"object\",\
  \ \"null\"],\n      \"description\": \"Settings to configure whether members can perform certain actions in the team\",\n      \"properties\": {\n        \"allowCreateUpdateChannels\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, members can add and update channels\"\n        },\n        \"allowCreatePrivateChannels\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, members can create private channels\"\n        },\n        \"allowDeleteChannels\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, members can delete channels\"\n        },\n        \"allowAddRemoveApps\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, members can add and remove apps\"\n        },\n        \"allowCreateUpdateRemoveTabs\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, members can create, update, and remove tabs\"\n        },\n        \"allowCreateUpdateRemoveConnectors\"\
  : {\n          \"type\": \"boolean\",\n          \"description\": \"If true, members can create, update, and remove connectors\"\n        }\n      }\n    },\n    \"TeamGuestSettings\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Settings to configure whether guests can perform certain actions in the team\",\n      \"properties\": {\n        \"allowCreateUpdateChannels\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, guests can create and update channels\"\n        },\n        \"allowDeleteChannels\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, guests can delete channels\"\n        }\n      }\n    },\n    \"TeamMessagingSettings\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Settings to configure messaging and mentions in the team\",\n      \"properties\": {\n        \"allowUserEditMessages\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, users can edit\
  \ their messages\"\n        },\n        \"allowUserDeleteMessages\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, users can delete their messages\"\n        },\n        \"allowOwnerDeleteMessages\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, owners can delete any message\"\n        },\n        \"allowTeamMentions\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, @team mentions are allowed\"\n        },\n        \"allowChannelMentions\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, @channel mentions are allowed\"\n        }\n      }\n    },\n    \"TeamFunSettings\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Settings to configure use of Giphy, memes, and stickers in the team\",\n      \"properties\": {\n        \"allowGiphy\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, enables Giphy use\"\n        },\n        \"\
  giphyContentRating\": {\n          \"type\": \"string\",\n          \"enum\": [\"moderate\", \"strict\"],\n          \"description\": \"Giphy content rating\"\n        },\n        \"allowStickersAndMemes\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, enables stickers and memes\"\n        },\n        \"allowCustomMemes\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, enables custom memes\"\n        }\n      }\n    },\n    \"TeamDiscoverySettings\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Settings to configure team discoverability by others\",\n      \"properties\": {\n        \"showInTeamsSearchAndSuggestions\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, team is visible in search and suggestions\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/json-schema/microsoft-teams-team-schema.json
tags: []
title: Microsoft Teams Team
---
