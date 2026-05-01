---
description: A marketing campaign in Oracle Eloqua used to orchestrate multi-channel communications including email marketing, lead nurturing, and multi-step engagement programs.
layout: schema
name: Eloqua Campaign
properties_list:
- description: Unique identifier for the campaign
  name: id
  type: string
- description: Asset type in Eloqua
  name: type
  type: string
- description: Campaign name
  name: name
  type: string
- description: Campaign description
  name: description
  type: string
- description: Current campaign status
  name: currentStatus
  type: string
- description: Campaign type - emailMarketing for simple campaigns, contact for multi-step campaigns
  name: campaignCategory
  type: string
- description: Campaign start date (Unix timestamp)
  name: startAt
  type: string
- description: Campaign end date (Unix timestamp)
  name: endAt
  type: string
- description: Number of members who entered the campaign in the last 90 days
  name: memberCount
  type: integer
- description: Whether the campaign is read-only
  name: isReadOnly
  type: boolean
- description: Whether members can re-enter the campaign
  name: isMemberAllowedReEntry
  type: boolean
- description: User identifier that the campaign runs as
  name: runAsUserId
  type: string
- description: Campaign canvas elements (steps, decisions, actions)
  name: elements
  type: array
- description: Containing folder identifier
  name: folderId
  type: string
- description: Level of detail returned for the campaign
  name: depth
  type: string
- description: Granted permissions on this campaign
  name: permissions
  type: array
- description: Creation timestamp (Unix time)
  name: createdAt
  type: string
- description: User login who created the campaign
  name: createdBy
  type: string
- description: Last update timestamp (Unix time)
  name: updatedAt
  type: string
- description: User login who last updated the campaign
  name: updatedBy
  type: string
provider_name: Oracle Eloqua
provider_slug: eloqua
schema_file: json-schema/eloqua-campaign-schema.json
slug: eloqua-campaign
source_filename: eloqua-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/en/cloud/saas/marketing/eloqua-rest-api/schemas/campaign.json\",\n  \"title\": \"Eloqua Campaign\",\n  \"description\": \"A marketing campaign in Oracle Eloqua used to orchestrate multi-channel communications including email marketing, lead nurturing, and multi-step engagement programs.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the campaign\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Asset type in Eloqua\",\n      \"const\": \"Campaign\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign name\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign description\"\
  \n    },\n    \"currentStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Draft\", \"Scheduled\", \"Completed\"],\n      \"description\": \"Current campaign status\",\n      \"readOnly\": true\n    },\n    \"campaignCategory\": {\n      \"type\": \"string\",\n      \"enum\": [\"emailMarketing\", \"contact\"],\n      \"description\": \"Campaign type - emailMarketing for simple campaigns, contact for multi-step campaigns\"\n    },\n    \"startAt\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign start date (Unix timestamp)\"\n    },\n    \"endAt\": {\n      \"type\": \"string\",\n      \"description\": \"Campaign end date (Unix timestamp)\"\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of members who entered the campaign in the last 90 days\",\n      \"readOnly\": true\n    },\n    \"isReadOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the campaign is\
  \ read-only\",\n      \"readOnly\": true\n    },\n    \"isMemberAllowedReEntry\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether members can re-enter the campaign\"\n    },\n    \"runAsUserId\": {\n      \"type\": \"string\",\n      \"description\": \"User identifier that the campaign runs as\"\n    },\n    \"elements\": {\n      \"type\": \"array\",\n      \"description\": \"Campaign canvas elements (steps, decisions, actions)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CampaignElement\"\n      }\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"Containing folder identifier\",\n      \"readOnly\": true\n    },\n    \"depth\": {\n      \"type\": \"string\",\n      \"enum\": [\"minimal\", \"partial\", \"complete\"],\n      \"description\": \"Level of detail returned for the campaign\",\n      \"readOnly\": true\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"Granted permissions on this campaign\"\
  ,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Creation timestamp (Unix time)\",\n      \"readOnly\": true\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User login who created the campaign\",\n      \"readOnly\": true\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Last update timestamp (Unix time)\",\n      \"readOnly\": true\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"User login who last updated the campaign\",\n      \"readOnly\": true\n    }\n  },\n  \"$defs\": {\n    \"CampaignElement\": {\n      \"type\": \"object\",\n      \"description\": \"An element on the campaign canvas such as a segment, email send step, wait step, or decision rule\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Element identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Element name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Element type (e.g., CampaignSegment, CampaignEmail, CampaignWaitAction)\"\n        },\n        \"memberCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of members at this step\",\n          \"readOnly\": true\n        },\n        \"outputTerminals\": {\n          \"type\": \"array\",\n          \"description\": \"Output connections to other elements\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\"\n              },\n              \"connectedId\": {\n                \"type\": \"string\",\n                \"description\": \"ID of the connected element\"\n              },\n              \"terminalId\": {\n               \
  \ \"type\": \"string\",\n                \"description\": \"Terminal identifier\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/json-schema/eloqua-campaign-schema.json
tags:
- CRM
- Email Marketing
- Lead Management
- Marketing Automation
title: Eloqua Campaign
---
