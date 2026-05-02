---
description: A community member in the Harbor platform representing a superfan who has joined a brand community, earns points through challenges and engagement, and can redeem rewards from the loyalty catalog.
layout: schema
name: Harbor Community Member
properties_list:
- description: Unique Harbor-assigned identifier for this community member.
  name: id
  type: string
- description: The brand's own user identifier used to link this Harbor member to the brand's platform account.
  name: externalId
  type: string
- description: Identifier of the Harbor community this member belongs to.
  name: communityId
  type: string
- description: The member's display name shown publicly in the community.
  name: displayName
  type: string
- description: The member's email address.
  name: email
  type: string
- description: The member's current point balance available for reward redemption.
  name: pointsBalance
  type: integer
- description: Lifetime total points earned by this member, used for tier qualification.
  name: totalPointsEarned
  type: integer
- description: ''
  name: tier
  type: object
- description: Unique referral code this member can share to earn referral bonus points when new members join using it.
  name: referralCode
  type: string
- description: Current membership status.
  name: status
  type: string
- description: Optional brand-defined metadata stored with this member record.
  name: metadata
  type: object
- description: ISO 8601 timestamp when this member joined the community.
  name: joinedAt
  type: string
- description: ISO 8601 timestamp of the member's most recent activity.
  name: lastActiveAt
  type: string
provider_name: Harbor
provider_slug: harbor
schema_file: json-schema/harbor-member-schema.json
slug: harbor-member
source_filename: harbor-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/harbor/blob/main/json-schema/harbor-member-schema.json\",\n  \"title\": \"Harbor Community Member\",\n  \"description\": \"A community member in the Harbor platform representing a superfan who has joined a brand community, earns points through challenges and engagement, and can redeem rewards from the loyalty catalog.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"externalId\", \"communityId\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Harbor-assigned identifier for this community member.\"\n    },\n    \"externalId\": {\n      \"type\": \"string\",\n      \"description\": \"The brand's own user identifier used to link this Harbor member to the brand's platform account.\"\n    },\n    \"communityId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the Harbor community\
  \ this member belongs to.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The member's display name shown publicly in the community.\",\n      \"maxLength\": 100\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The member's email address.\"\n    },\n    \"pointsBalance\": {\n      \"type\": \"integer\",\n      \"description\": \"The member's current point balance available for reward redemption.\",\n      \"minimum\": 0\n    },\n    \"totalPointsEarned\": {\n      \"type\": \"integer\",\n      \"description\": \"Lifetime total points earned by this member, used for tier qualification.\",\n      \"minimum\": 0\n    },\n    \"tier\": {\n      \"$ref\": \"#/$defs/Tier\"\n    },\n    \"referralCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique referral code this member can share to earn referral bonus points when new members join using it.\"\n    },\n    \"status\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Current membership status.\",\n      \"enum\": [\"active\", \"inactive\", \"banned\"]\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Optional brand-defined metadata stored with this member record.\",\n      \"additionalProperties\": true\n    },\n    \"joinedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when this member joined the community.\"\n    },\n    \"lastActiveAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the member's most recent activity.\"\n    }\n  },\n  \"$defs\": {\n    \"Tier\": {\n      \"type\": \"object\",\n      \"title\": \"Tier\",\n      \"description\": \"A loyalty tier that members progress through as they earn lifetime points.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Unique tier identifier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Tier display name shown to members (e.g., Bronze, Silver, Gold, Platinum).\"\n        },\n        \"pointsRequired\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum lifetime points required to qualify for this tier.\",\n          \"minimum\": 0\n        },\n        \"benefits\": {\n          \"type\": \"array\",\n          \"description\": \"List of benefit descriptions associated with this tier.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable benefit description.\"\n          }\n        }\n      }\n    },\n    \"PointTransaction\": {\n      \"type\": \"object\",\n      \"title\": \"PointTransaction\",\n      \"description\": \"A single point earning or spending transaction for a community member.\",\n      \"required\": [\"type\", \"points\"\
  , \"description\", \"createdAt\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique transaction identifier.\"\n        },\n        \"memberId\": {\n          \"type\": \"string\",\n          \"description\": \"Member identifier this transaction belongs to.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Transaction type indicating whether points were earned or spent.\",\n          \"enum\": [\"earn\", \"spend\", \"adjustment\", \"expiry\"]\n        },\n        \"points\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of points in this transaction. Positive for earnings, negative for spending.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the transaction source.\"\n        },\n        \"challengeId\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Reference to the challenge that triggered this transaction, if applicable.\"\n        },\n        \"redemptionId\": {\n          \"type\": \"string\",\n          \"description\": \"Reference to the redemption that triggered this transaction, if applicable.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the transaction.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/harbor/refs/heads/main/json-schema/harbor-member-schema.json
tags:
- Community
- Engagement
- Loyalty
- Superfans
title: Harbor Community Member
---
