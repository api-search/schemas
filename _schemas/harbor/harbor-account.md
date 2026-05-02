---
description: A Harbor community platform account representing a superfan user with linked identities, resources, and guild memberships.
layout: schema
name: Harbor Account
properties_list:
- description: Unique account identifier
  name: id
  type: string
- description: Display name shown in the community
  name: username
  type: string
- description: Primary email address for the account
  name: email
  type: string
- description: External platform identities linked to this account
  name: identities
  type: array
- description: Map of resource type names to current totals (e.g., points, badges)
  name: resources
  type: object
- description: Guild memberships for this account
  name: guilds
  type: array
- description: Moderation strike records
  name: strikes
  type: array
- description: ISO 8601 timestamp when the account was created
  name: createdAt
  type: string
- description: ISO 8601 timestamp of the last account update
  name: updatedAt
  type: string
provider_name: Harbor
provider_slug: harbor
schema_file: json-schema/harbor-account-schema.json
slug: harbor-account
source_filename: harbor-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.harbor.gg/schemas/harbor/account.json\",\n  \"title\": \"Harbor Account\",\n  \"description\": \"A Harbor community platform account representing a superfan user with linked identities, resources, and guild memberships.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique account identifier\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"maxLength\": 64,\n      \"description\": \"Display name shown in the community\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address for the account\"\n    },\n    \"identities\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Identity\" },\n      \"description\": \"External platform identities linked to this account\"\n    },\n\
  \    \"resources\": {\n      \"type\": \"object\",\n      \"additionalProperties\": { \"type\": \"number\" },\n      \"description\": \"Map of resource type names to current totals (e.g., points, badges)\"\n    },\n    \"guilds\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/GuildMembership\" },\n      \"description\": \"Guild memberships for this account\"\n    },\n    \"strikes\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/AccountStrike\" },\n      \"description\": \"Moderation strike records\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the account was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last account update\"\n    }\n  },\n  \"$defs\": {\n    \"Identity\": {\n      \"type\": \"object\",\n      \"required\": [\"id\", \"\
  type\", \"externalId\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Identity record identifier\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"discord\", \"steam\", \"ethereum\", \"aptos\", \"beamable\", \"youtube\", \"twitch\"],\n          \"description\": \"Identity provider type\"\n        },\n        \"externalId\": {\n          \"type\": \"string\",\n          \"description\": \"User identifier from the external platform\"\n        },\n        \"externalUsername\": {\n          \"type\": \"string\",\n          \"description\": \"Display name on the external platform\"\n        },\n        \"linkedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When this identity was linked to the account\"\n        }\n      }\n    },\n    \"GuildMembership\": {\n      \"type\": \"object\",\n      \"required\": [\"guildId\"],\n    \
  \  \"properties\": {\n        \"guildId\": {\n          \"type\": \"string\",\n          \"description\": \"Guild identifier\"\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"enum\": [\"member\", \"owner\"],\n          \"description\": \"Member's role within the guild\"\n        },\n        \"joinedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the account joined the guild\"\n        }\n      }\n    },\n    \"AccountStrike\": {\n      \"type\": \"object\",\n      \"required\": [\"id\", \"accountId\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Strike record identifier\"\n        },\n        \"accountId\": {\n          \"type\": \"string\",\n          \"description\": \"Account that received the strike\"\n        },\n        \"reason\": {\n          \"type\": \"string\",\n          \"description\": \"Reason for the moderation action\"\
  \n        },\n        \"issuedBy\": {\n          \"type\": \"string\",\n          \"description\": \"Admin account ID that issued the strike\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the strike was issued\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/json-schema/harbor-account-schema.json
tags:
- Community
- Engagement
- Loyalty
- Superfans
title: Harbor Account
---
