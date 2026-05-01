---
description: Schema for a Google Ads campaign resource. A campaign is the top-level organizational unit in Google Ads that groups ad groups and sets budgets, bidding strategies, targeting criteria, and advertising channel types. Campaigns control how and where ads are shown across Google Search, Display Network, YouTube, Shopping, and other channels.
layout: schema
name: Google Ads Campaign
properties_list:
- description: The resource name of the campaign in the format customers/{customerId}/campaigns/{campaignId}.
  name: resourceName
  type: string
- description: The unique ID of the campaign. Assigned by Google Ads upon creation.
  name: id
  type: integer
- description: The name of the campaign. Must be unique across all active and paused campaigns within the account. Maximum 255 characters.
  name: name
  type: string
- description: The serving status of the campaign. ENABLED campaigns are actively serving ads. PAUSED campaigns retain their configuration but do not serve. REMOVED campaigns are permanently deleted.
  name: status
  type: string
- description: The primary advertising channel type that determines where ads can appear. SEARCH serves text ads on Google Search. DISPLAY serves image and text ads across the Google Display Network. PERFORMANCE_MAX
  name: advertisingChannelType
  type: string
- description: Optional refinement of the advertising channel type providing more specific campaign behavior.
  name: advertisingChannelSubType
  type: string
- description: Resource name of the campaign budget in the format customers/{customerId}/campaignBudgets/{budgetId}.
  name: campaignBudget
  type: string
- description: The type of bidding strategy used by the campaign. TARGET_CPA optimizes for a target cost per acquisition. MAXIMIZE_CONVERSIONS uses machine learning to maximize total conversions. MANUAL_CPC gives fu
  name: biddingStrategyType
  type: string
- description: Resource name of a portfolio bidding strategy shared across campaigns.
  name: biddingStrategy
  type: string
- description: The start date of the campaign in yyyy-MM-dd format. If not set, the campaign starts immediately upon enabling.
  name: startDate
  type: string
- description: The end date of the campaign in yyyy-MM-dd format. If not set, the campaign runs indefinitely.
  name: endDate
  type: string
- description: The actual serving status of the campaign taking into account budget, schedule, and approval status.
  name: servingStatus
  type: string
- description: Network targeting settings that determine which Google networks the ads appear on.
  name: networkSettings
  type: object
- description: Target CPA (cost per acquisition) bidding strategy settings.
  name: targetCpa
  type: object
- description: Target ROAS (return on ad spend) bidding strategy settings.
  name: targetRoas
  type: object
- description: Maximize Conversions bidding strategy settings.
  name: maximizeConversions
  type: object
- description: Maximize Conversion Value bidding strategy settings.
  name: maximizeConversionValue
  type: object
- description: Manual CPC (cost per click) bidding strategy settings.
  name: manualCpc
  type: object
- description: Target Spend bidding strategy settings for maximizing clicks within a budget.
  name: targetSpend
  type: object
- description: Target Impression Share bidding strategy settings.
  name: targetImpressionShare
  type: object
- description: Settings for geographic targeting behavior.
  name: geoTargetTypeSetting
  type: object
- description: Resource names of labels applied to this campaign for organization and filtering.
  name: labels
  type: array
- description: Optimization score as a value between 0 and 1 indicating how well the campaign is set up relative to Google's best practices.
  name: optimizationScore
  type: number
- description: Custom URL parameters for tracking.
  name: urlCustomParameters
  type: array
- description: URL template for constructing tracking URLs with ValueTrack parameters.
  name: trackingUrlTemplate
  type: string
- description: Suffix appended to final URLs for additional tracking parameters.
  name: finalUrlSuffix
  type: string
- description: The payment mode for the campaign determining what is billed.
  name: paymentMode
  type: string
- description: Whether this is a base campaign, draft, or experiment.
  name: experimentType
  type: string
- description: Resource name of the base campaign for drafts and experiments.
  name: baseCampaign
  type: string
provider_name: Google Ads
provider_slug: google-ads
schema_file: json-schema/google-ads-campaign-schema.json
slug: google-ads-campaign
source_filename: google-ads-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/json-schema/google-ads-campaign-schema.json\",\n  \"title\": \"Google Ads Campaign\",\n  \"description\": \"Schema for a Google Ads campaign resource. A campaign is the top-level organizational unit in Google Ads that groups ad groups and sets budgets, bidding strategies, targeting criteria, and advertising channel types. Campaigns control how and where ads are shown across Google Search, Display Network, YouTube, Shopping, and other channels.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"advertisingChannelType\"],\n  \"properties\": {\n    \"resourceName\": {\n      \"type\": \"string\",\n      \"pattern\": \"^customers/\\\\d+/campaigns/\\\\d+$\",\n      \"description\": \"The resource name of the campaign in the format customers/{customerId}/campaigns/{campaignId}.\"\n    },\n    \"id\": {\n      \"type\"\
  : \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The unique ID of the campaign. Assigned by Google Ads upon creation.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"The name of the campaign. Must be unique across all active and paused campaigns within the account. Maximum 255 characters.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"ENABLED\", \"PAUSED\", \"REMOVED\", \"UNKNOWN\", \"UNSPECIFIED\"],\n      \"description\": \"The serving status of the campaign. ENABLED campaigns are actively serving ads. PAUSED campaigns retain their configuration but do not serve. REMOVED campaigns are permanently deleted.\"\n    },\n    \"advertisingChannelType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SEARCH\",\n        \"DISPLAY\",\n        \"SHOPPING\",\n        \"VIDEO\",\n        \"MULTI_CHANNEL\",\n        \"LOCAL\",\n        \"SMART\",\n        \"PERFORMANCE_MAX\"\
  ,\n        \"DEMAND_GEN\",\n        \"TRAVEL\",\n        \"LOCAL_SERVICES\",\n        \"UNKNOWN\",\n        \"UNSPECIFIED\"\n      ],\n      \"description\": \"The primary advertising channel type that determines where ads can appear. SEARCH serves text ads on Google Search. DISPLAY serves image and text ads across the Google Display Network. PERFORMANCE_MAX uses automation across all Google channels.\"\n    },\n    \"advertisingChannelSubType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SEARCH_MOBILE_APP\",\n        \"DISPLAY_MOBILE_APP\",\n        \"SEARCH_EXPRESS\",\n        \"DISPLAY_EXPRESS\",\n        \"SHOPPING_SMART_ADS\",\n        \"DISPLAY_GMAIL_AD\",\n        \"DISPLAY_SMART_CAMPAIGN\",\n        \"VIDEO_OUTSTREAM\",\n        \"VIDEO_ACTION\",\n        \"VIDEO_NON_SKIPPABLE\",\n        \"VIDEO_REACH_TARGET_FREQUENCY\",\n        \"APP_CAMPAIGN\",\n        \"APP_CAMPAIGN_FOR_ENGAGEMENT\",\n        \"LOCAL_CAMPAIGN\",\n        \"SHOPPING_COMPARISON_LISTING_ADS\"\
  ,\n        \"SMART_CAMPAIGN\",\n        \"VIDEO_SEQUENCE\",\n        \"APP_CAMPAIGN_FOR_PRE_REGISTRATION\",\n        \"TRAVEL_ACTIVITIES\",\n        \"UNKNOWN\",\n        \"UNSPECIFIED\"\n      ],\n      \"description\": \"Optional refinement of the advertising channel type providing more specific campaign behavior.\"\n    },\n    \"campaignBudget\": {\n      \"type\": \"string\",\n      \"pattern\": \"^customers/\\\\d+/campaignBudgets/\\\\d+$\",\n      \"description\": \"Resource name of the campaign budget in the format customers/{customerId}/campaignBudgets/{budgetId}.\"\n    },\n    \"biddingStrategyType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TARGET_CPA\",\n        \"TARGET_ROAS\",\n        \"TARGET_SPEND\",\n        \"MAXIMIZE_CONVERSIONS\",\n        \"MAXIMIZE_CONVERSION_VALUE\",\n        \"MANUAL_CPC\",\n        \"MANUAL_CPM\",\n        \"MANUAL_CPV\",\n        \"TARGET_IMPRESSION_SHARE\",\n        \"ENHANCED_CPC\",\n        \"UNKNOWN\",\n        \"UNSPECIFIED\"\
  \n      ],\n      \"description\": \"The type of bidding strategy used by the campaign. TARGET_CPA optimizes for a target cost per acquisition. MAXIMIZE_CONVERSIONS uses machine learning to maximize total conversions. MANUAL_CPC gives full control over individual keyword bids.\"\n    },\n    \"biddingStrategy\": {\n      \"type\": \"string\",\n      \"pattern\": \"^customers/\\\\d+/biddingStrategies/\\\\d+$\",\n      \"description\": \"Resource name of a portfolio bidding strategy shared across campaigns.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{4}-\\\\d{2}-\\\\d{2}$\",\n      \"description\": \"The start date of the campaign in yyyy-MM-dd format. If not set, the campaign starts immediately upon enabling.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{4}-\\\\d{2}-\\\\d{2}$\",\n      \"description\": \"The end date of the campaign in yyyy-MM-dd format. If not set, the campaign runs indefinitely.\"\n\
  \    },\n    \"servingStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SERVING\",\n        \"NONE\",\n        \"ENDED\",\n        \"PENDING\",\n        \"SUSPENDED\",\n        \"UNKNOWN\",\n        \"UNSPECIFIED\"\n      ],\n      \"description\": \"The actual serving status of the campaign taking into account budget, schedule, and approval status.\"\n    },\n    \"networkSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Network targeting settings that determine which Google networks the ads appear on.\",\n      \"properties\": {\n        \"targetGoogleSearch\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether ads are served on the Google Search Network (google.com and search partners).\"\n        },\n        \"targetSearchNetwork\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether ads are served on Google search partner sites.\"\n        },\n        \"targetContentNetwork\": {\n          \"type\"\
  : \"boolean\",\n          \"description\": \"Whether ads are served on the Google Display Network.\"\n        },\n        \"targetPartnerSearchNetwork\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether ads are served on the Google Partner Search Network.\"\n        }\n      }\n    },\n    \"targetCpa\": {\n      \"type\": \"object\",\n      \"description\": \"Target CPA (cost per acquisition) bidding strategy settings.\",\n      \"properties\": {\n        \"targetCpaMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"minimum\": 0,\n          \"description\": \"Target CPA amount in micros. One million micros equals one unit of currency (e.g., 1,500,000 micros = $1.50 USD).\"\n        },\n        \"cpcBidCeilingMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum CPC bid ceiling in micros for the strategy.\"\n        },\n        \"cpcBidFloorMicros\": {\n  \
  \        \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Minimum CPC bid floor in micros for the strategy.\"\n        }\n      }\n    },\n    \"targetRoas\": {\n      \"type\": \"object\",\n      \"description\": \"Target ROAS (return on ad spend) bidding strategy settings.\",\n      \"properties\": {\n        \"targetRoas\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Target return on ad spend as a ratio. For example, 3.5 means a 350% return on ad spend.\"\n        },\n        \"cpcBidCeilingMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum CPC bid ceiling in micros.\"\n        },\n        \"cpcBidFloorMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Minimum CPC bid floor in micros.\"\n        }\n      }\n    },\n    \"maximizeConversions\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Maximize Conversions bidding strategy settings.\",\n      \"properties\": {\n        \"targetCpaMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Optional target CPA in micros when using maximize conversions with a CPA goal.\"\n        },\n        \"cpcBidCeilingMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum CPC bid ceiling in micros.\"\n        },\n        \"cpcBidFloorMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Minimum CPC bid floor in micros.\"\n        }\n      }\n    },\n    \"maximizeConversionValue\": {\n      \"type\": \"object\",\n      \"description\": \"Maximize Conversion Value bidding strategy settings.\",\n      \"properties\": {\n        \"targetRoas\": {\n          \"type\": \"number\",\n          \"description\": \"Optional target ROAS when using maximize\
  \ conversion value.\"\n        },\n        \"cpcBidCeilingMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum CPC bid ceiling in micros.\"\n        },\n        \"cpcBidFloorMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Minimum CPC bid floor in micros.\"\n        }\n      }\n    },\n    \"manualCpc\": {\n      \"type\": \"object\",\n      \"description\": \"Manual CPC (cost per click) bidding strategy settings.\",\n      \"properties\": {\n        \"enhancedCpcEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether Enhanced CPC is enabled, allowing Google to automatically adjust bids for clicks more likely to convert.\"\n        }\n      }\n    },\n    \"targetSpend\": {\n      \"type\": \"object\",\n      \"description\": \"Target Spend bidding strategy settings for maximizing clicks within a budget.\",\n      \"properties\": {\n\
  \        \"targetSpendMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Target spend amount in micros.\"\n        },\n        \"cpcBidCeilingMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum CPC bid ceiling in micros.\"\n        }\n      }\n    },\n    \"targetImpressionShare\": {\n      \"type\": \"object\",\n      \"description\": \"Target Impression Share bidding strategy settings.\",\n      \"properties\": {\n        \"location\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ANYWHERE_ON_PAGE\",\n            \"TOP_OF_PAGE\",\n            \"ABSOLUTE_TOP_OF_PAGE\",\n            \"UNKNOWN\",\n            \"UNSPECIFIED\"\n          ],\n          \"description\": \"Target location on the search results page.\"\n        },\n        \"locationFractionMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n     \
  \     \"description\": \"Target fraction of impressions in the chosen location (in micros, e.g., 700000 = 70%).\"\n        },\n        \"cpcBidCeilingMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum CPC bid ceiling in micros.\"\n        }\n      }\n    },\n    \"geoTargetTypeSetting\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for geographic targeting behavior.\",\n      \"properties\": {\n        \"positiveGeoTargetType\": {\n          \"type\": \"string\",\n          \"enum\": [\"PRESENCE_OR_INTEREST\", \"SEARCH_INTEREST\", \"PRESENCE\"],\n          \"description\": \"How positive geo targeting is applied. PRESENCE targets users physically in the location. SEARCH_INTEREST targets users searching for the location. PRESENCE_OR_INTEREST targets both.\"\n        },\n        \"negativeGeoTargetType\": {\n          \"type\": \"string\",\n          \"enum\": [\"PRESENCE_OR_INTEREST\", \"PRESENCE\"],\n\
  \          \"description\": \"How negative geo targeting is applied to exclude locations.\"\n        }\n      }\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Resource names of labels applied to this campaign for organization and filtering.\"\n    },\n    \"optimizationScore\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Optimization score as a value between 0 and 1 indicating how well the campaign is set up relative to Google's best practices.\"\n    },\n    \"urlCustomParameters\": {\n      \"type\": \"array\",\n      \"description\": \"Custom URL parameters for tracking.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The custom parameter key.\"\n          },\n          \"value\": {\n            \"type\": \"string\"\
  ,\n            \"description\": \"The custom parameter value.\"\n          }\n        }\n      }\n    },\n    \"trackingUrlTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"URL template for constructing tracking URLs with ValueTrack parameters.\"\n    },\n    \"finalUrlSuffix\": {\n      \"type\": \"string\",\n      \"description\": \"Suffix appended to final URLs for additional tracking parameters.\"\n    },\n    \"paymentMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CLICKS\",\n        \"CONVERSION_VALUE\",\n        \"CONVERSIONS\",\n        \"GUEST_STAY\",\n        \"UNKNOWN\",\n        \"UNSPECIFIED\"\n      ],\n      \"description\": \"The payment mode for the campaign determining what is billed.\"\n    },\n    \"experimentType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"BASE\",\n        \"DRAFT\",\n        \"EXPERIMENT\",\n        \"UNKNOWN\",\n        \"UNSPECIFIED\"\n      ],\n      \"description\": \"Whether this is\
  \ a base campaign, draft, or experiment.\"\n    },\n    \"baseCampaign\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the base campaign for drafts and experiments.\"\n    }\n  },\n  \"$defs\": {\n    \"CampaignBudget\": {\n      \"type\": \"object\",\n      \"description\": \"A budget that defines spending limits for one or more campaigns.\",\n      \"properties\": {\n        \"resourceName\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the campaign budget.\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"The unique ID of the campaign budget.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the campaign budget.\"\n        },\n        \"amountMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"minimum\": 0,\n          \"description\": \"Daily\
  \ budget amount in micros. One million micros equals one unit of currency.\"\n        },\n        \"totalAmountMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Lifetime total budget amount in micros.\"\n        },\n        \"deliveryMethod\": {\n          \"type\": \"string\",\n          \"enum\": [\"STANDARD\", \"ACCELERATED\", \"UNKNOWN\", \"UNSPECIFIED\"],\n          \"description\": \"How the budget is spent. STANDARD distributes spending evenly. ACCELERATED spends budget as quickly as possible.\"\n        },\n        \"explicitlyShared\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this budget is shared across multiple campaigns.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"ENABLED\", \"REMOVED\", \"UNKNOWN\", \"UNSPECIFIED\"],\n          \"description\": \"The status of the campaign budget.\"\n        }\n      }\n    },\n    \"AdGroup\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"An ad group within the campaign containing a set of ads and targeting criteria.\",\n      \"properties\": {\n        \"resourceName\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the ad group.\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"The unique ID of the ad group.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the ad group.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"ENABLED\", \"PAUSED\", \"REMOVED\", \"UNKNOWN\", \"UNSPECIFIED\"],\n          \"description\": \"The status of the ad group.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SEARCH_STANDARD\",\n            \"DISPLAY_STANDARD\",\n            \"SHOPPING_PRODUCT_ADS\",\n        \
  \    \"VIDEO_TRUE_VIEW_IN_STREAM\",\n            \"VIDEO_BUMPER\",\n            \"HOTEL_ADS\",\n            \"UNKNOWN\",\n            \"UNSPECIFIED\"\n          ],\n          \"description\": \"The type of the ad group.\"\n        },\n        \"cpcBidMicros\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum CPC bid in micros at the ad group level.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/json-schema/google-ads-campaign-schema.json
tags:
- Advertising
- Campaign Management
- Digital Advertising
- Google
- Marketing
- PPC
title: Google Ads Campaign
---
