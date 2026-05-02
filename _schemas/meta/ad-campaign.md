---
description: Represents an advertising campaign in the Meta Marketing API (Campaign level in the Campaign > Ad Set > Ad hierarchy). Includes budget, objective, status, and scheduling fields.
layout: schema
name: Meta Marketing API Ad Campaign
properties_list:
- description: The unique identifier for the campaign.
  name: id
  type: string
- description: The name of the campaign.
  name: name
  type: string
- description: The ID of the ad account that owns the campaign.
  name: account_id
  type: string
- description: The campaign objective defining the optimization goal. Uses the Outcome-Based Ads objectives introduced in Meta Marketing API v18+.
  name: objective
  type: string
- description: The campaign status set by the advertiser.
  name: status
  type: string
- description: The effective status of the campaign, accounting for parent ad account status and any issues.
  name: effective_status
  type: string
- description: The configured status of the campaign as set in the API.
  name: configured_status
  type: string
- description: The buying type for the campaign. AUCTION is the default for most campaigns.
  name: buying_type
  type: string
- description: The bid strategy for the campaign.
  name: bid_strategy
  type: string
- description: The remaining budget of the campaign in the account currency, expressed in cents.
  name: budget_remaining
  type: string
- description: The daily budget of the campaign in the account currency, expressed in cents.
  name: daily_budget
  type: string
- description: The lifetime budget of the campaign in the account currency, expressed in cents.
  name: lifetime_budget
  type: string
- description: The spend cap for the campaign in the account currency, expressed in cents.
  name: spend_cap
  type: string
- description: Special ad categories the campaign falls under (e.g. credit, employment, housing, social issues).
  name: special_ad_categories
  type: array
- description: The start time of the campaign, in ISO 8601 format.
  name: start_time
  type: string
- description: The stop/end time of the campaign, in ISO 8601 format.
  name: stop_time
  type: string
- description: The time the campaign was created, in ISO 8601 format.
  name: created_time
  type: string
- description: The time the campaign was last updated, in ISO 8601 format.
  name: updated_time
  type: string
- description: The ID of the source campaign this was copied from, if applicable.
  name: source_campaign_id
  type: string
- description: The type of smart promotion applied to the campaign.
  name: smart_promotion_type
  type: string
- description: The pacing type for ad delivery.
  name: pacing_type
  type: array
- description: The object being promoted (e.g. a pixel, app, or Page).
  name: promoted_object
  type: object
- description: The ad sets within this campaign.
  name: adsets
  type: object
- description: Performance insights/metrics for the campaign.
  name: insights
  type: object
provider_name: Meta
provider_slug: meta
schema_file: json-schema/ad-campaign.json
slug: ad-campaign
source_filename: ad-campaign.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://meta.com/schemas/marketing-api/ad-campaign.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Meta Marketing API Ad Campaign\",\n  \"description\": \"Represents an advertising campaign in the Meta Marketing API (Campaign level in the Campaign > Ad Set > Ad hierarchy). Includes budget, objective, status, and scheduling fields.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the campaign.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the campaign.\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the ad account that owns the campaign.\"\n    },\n    \"objective\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OUTCOME_AWARENESS\",\n        \"OUTCOME_ENGAGEMENT\"\
  ,\n        \"OUTCOME_LEADS\",\n        \"OUTCOME_SALES\",\n        \"OUTCOME_TRAFFIC\",\n        \"OUTCOME_APP_PROMOTION\"\n      ],\n      \"description\": \"The campaign objective defining the optimization goal. Uses the Outcome-Based Ads objectives introduced in Meta Marketing API v18+.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"PAUSED\",\n        \"DELETED\",\n        \"ARCHIVED\"\n      ],\n      \"description\": \"The campaign status set by the advertiser.\"\n    },\n    \"effective_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"PAUSED\",\n        \"DELETED\",\n        \"ARCHIVED\",\n        \"IN_PROCESS\",\n        \"WITH_ISSUES\",\n        \"CAMPAIGN_PAUSED\"\n      ],\n      \"description\": \"The effective status of the campaign, accounting for parent ad account status and any issues.\"\n    },\n    \"configured_status\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\n        \"ACTIVE\",\n        \"PAUSED\",\n        \"DELETED\",\n        \"ARCHIVED\"\n      ],\n      \"description\": \"The configured status of the campaign as set in the API.\"\n    },\n    \"buying_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AUCTION\",\n        \"RESERVED\"\n      ],\n      \"description\": \"The buying type for the campaign. AUCTION is the default for most campaigns.\"\n    },\n    \"bid_strategy\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LOWEST_COST_WITHOUT_CAP\",\n        \"LOWEST_COST_WITH_BID_CAP\",\n        \"COST_CAP\",\n        \"LOWEST_COST_WITH_MIN_ROAS\"\n      ],\n      \"description\": \"The bid strategy for the campaign.\"\n    },\n    \"budget_remaining\": {\n      \"type\": \"string\",\n      \"description\": \"The remaining budget of the campaign in the account currency, expressed in cents.\"\n    },\n    \"daily_budget\": {\n      \"type\": \"string\",\n      \"description\": \"The daily budget of\
  \ the campaign in the account currency, expressed in cents.\"\n    },\n    \"lifetime_budget\": {\n      \"type\": \"string\",\n      \"description\": \"The lifetime budget of the campaign in the account currency, expressed in cents.\"\n    },\n    \"spend_cap\": {\n      \"type\": \"string\",\n      \"description\": \"The spend cap for the campaign in the account currency, expressed in cents.\"\n    },\n    \"special_ad_categories\": {\n      \"type\": \"array\",\n      \"description\": \"Special ad categories the campaign falls under (e.g. credit, employment, housing, social issues).\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"NONE\",\n          \"EMPLOYMENT\",\n          \"HOUSING\",\n          \"CREDIT\",\n          \"ISSUES_ELECTIONS_POLITICS\"\n        ]\n      }\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The start time of the campaign, in ISO 8601 format.\"\n\
  \    },\n    \"stop_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The stop/end time of the campaign, in ISO 8601 format.\"\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the campaign was created, in ISO 8601 format.\"\n    },\n    \"updated_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the campaign was last updated, in ISO 8601 format.\"\n    },\n    \"source_campaign_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the source campaign this was copied from, if applicable.\"\n    },\n    \"smart_promotion_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of smart promotion applied to the campaign.\"\n    },\n    \"pacing_type\": {\n      \"type\": \"array\",\n      \"description\": \"The pacing type for ad delivery.\",\n      \"items\": {\n   \
  \     \"type\": \"string\",\n        \"enum\": [\n          \"standard\",\n          \"no_pacing\",\n          \"day_parting\"\n        ]\n      }\n    },\n    \"promoted_object\": {\n      \"type\": \"object\",\n      \"description\": \"The object being promoted (e.g. a pixel, app, or Page).\",\n      \"properties\": {\n        \"pixel_id\": {\n          \"type\": \"string\",\n          \"description\": \"The Meta Pixel ID.\"\n        },\n        \"application_id\": {\n          \"type\": \"string\",\n          \"description\": \"The application (app) ID.\"\n        },\n        \"page_id\": {\n          \"type\": \"string\",\n          \"description\": \"The Facebook Page ID.\"\n        },\n        \"custom_event_type\": {\n          \"type\": \"string\",\n          \"description\": \"The custom conversion event type (e.g. PURCHASE, LEAD, ADD_TO_CART).\"\n        }\n      }\n    },\n    \"adsets\": {\n      \"type\": \"object\",\n      \"description\": \"The ad sets within this campaign.\"\
  ,\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"status\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"insights\": {\n      \"type\": \"object\",\n      \"description\": \"Performance insights/metrics for the campaign.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"impressions\": {\n                \"type\": \"string\"\n              },\n              \"clicks\": {\n                \"type\": \"string\"\n              },\n              \"spend\": {\n                \"type\": \"\
  string\"\n              },\n              \"reach\": {\n                \"type\": \"string\"\n              },\n              \"cpc\": {\n                \"type\": \"string\"\n              },\n              \"cpm\": {\n                \"type\": \"string\"\n              },\n              \"ctr\": {\n                \"type\": \"string\"\n              },\n              \"date_start\": {\n                \"type\": \"string\",\n                \"format\": \"date\"\n              },\n              \"date_stop\": {\n                \"type\": \"string\",\n                \"format\": \"date\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"id\": \"23851234567890123\",\n      \"name\": \"Summer Sale 2025 - Awareness\",\n      \"account_id\": \"act_123456789\",\n      \"objective\": \"OUTCOME_AWARENESS\",\n      \"status\": \"ACTIVE\",\n      \"effective_status\": \"ACTIVE\",\n      \"buying_type\"\
  : \"AUCTION\",\n      \"bid_strategy\": \"LOWEST_COST_WITHOUT_CAP\",\n      \"daily_budget\": \"5000\",\n      \"special_ad_categories\": [\n        \"NONE\"\n      ],\n      \"start_time\": \"2025-06-01T00:00:00-0700\",\n      \"created_time\": \"2025-05-28T10:15:00-0700\",\n      \"promoted_object\": {\n        \"page_id\": \"123456789012345\"\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/json-schema/ad-campaign.json
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
title: Meta Marketing API Ad Campaign
---
