---
description: A Mailchimp email marketing campaign. Represents a single email send or series of emails targeted at a list or segment of subscribers. Campaigns can be regular, plain-text, A/B split, RSS-driven, or multivariate.
layout: schema
name: Mailchimp Campaign
properties_list:
- description: A string that uniquely identifies this campaign.
  name: id
  type: string
- description: The ID used in the Mailchimp web application.
  name: web_id
  type: integer
- description: If this campaign is the child of another campaign, this identifies the parent campaign. For example, for RSS or Automation children.
  name: parent_campaign_id
  type: string
- description: The type of campaign.
  name: type
  type: string
- description: The date and time the campaign was created in ISO 8601 format.
  name: create_time
  type: string
- description: The link to the campaign's archive version.
  name: archive_url
  type: string
- description: The original link to the campaign's archive version.
  name: long_archive_url
  type: string
- description: The current status of the campaign.
  name: status
  type: string
- description: The total number of emails sent for this campaign.
  name: emails_sent
  type: integer
- description: The date and time a campaign was sent in ISO 8601 format.
  name: send_time
  type: string
- description: How the campaign's content is put together.
  name: content_type
  type: string
- description: Deprecated. Whether the campaign needs its blocks refreshed by opening the web-based campaign editor. Will always return false.
  name: needs_block_refresh
  type: boolean
- description: Whether the campaign qualifies to be resent to non-openers.
  name: resendable
  type: boolean
- description: List/audience settings for the campaign.
  name: recipients
  type: object
- description: The settings for the campaign, including subject line, from name, and reply-to address.
  name: settings
  type: object
- description: The tracking options for a campaign.
  name: tracking
  type: object
- description: For sent campaigns, a summary of opens, clicks, and e-commerce data.
  name: report_summary
  type: object
- description: Updates on campaigns in the process of sending.
  name: delivery_status
  type: object
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/campaign.json
slug: campaign
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/messaging/mailchimp/json-schema/campaign.json\",\n  \"title\": \"Mailchimp Campaign\",\n  \"description\": \"A Mailchimp email marketing campaign. Represents a single email send or series of emails targeted at a list or segment of subscribers. Campaigns can be regular, plain-text, A/B split, RSS-driven, or multivariate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A string that uniquely identifies this campaign.\",\n      \"readOnly\": true\n    },\n    \"web_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID used in the Mailchimp web application.\",\n      \"readOnly\": true\n    },\n    \"parent_campaign_id\": {\n      \"type\": \"string\",\n      \"description\": \"If this campaign is the child of another campaign, this identifies the parent campaign. For example, for\
  \ RSS or Automation children.\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of campaign.\",\n      \"enum\": [\"regular\", \"plaintext\", \"absplit\", \"rss\", \"variate\"]\n    },\n    \"create_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the campaign was created in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"archive_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The link to the campaign's archive version.\",\n      \"readOnly\": true\n    },\n    \"long_archive_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The original link to the campaign's archive version.\",\n      \"readOnly\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the campaign.\",\n      \"enum\": [\"save\", \"\
  paused\", \"schedule\", \"sending\", \"sent\", \"canceled\", \"canceling\", \"archived\"],\n      \"readOnly\": true\n    },\n    \"emails_sent\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of emails sent for this campaign.\",\n      \"readOnly\": true\n    },\n    \"send_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time a campaign was sent in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"How the campaign's content is put together.\",\n      \"enum\": [\"template\", \"html\", \"url\", \"multichannel\"]\n    },\n    \"needs_block_refresh\": {\n      \"type\": \"boolean\",\n      \"description\": \"Deprecated. Whether the campaign needs its blocks refreshed by opening the web-based campaign editor. Will always return false.\",\n      \"readOnly\": true\n    },\n    \"resendable\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether the campaign qualifies to be resent to non-openers.\",\n      \"readOnly\": true\n    },\n    \"recipients\": {\n      \"type\": \"object\",\n      \"description\": \"List/audience settings for the campaign.\",\n      \"properties\": {\n        \"list_id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique list/audience ID.\"\n        },\n        \"list_is_active\": {\n          \"type\": \"boolean\",\n          \"description\": \"The status of the list used, namely if it's deleted or disabled.\",\n          \"readOnly\": true\n        },\n        \"list_name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the list/audience.\",\n          \"readOnly\": true\n        },\n        \"segment_text\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the segment used for the campaign, formatted as HTML.\",\n          \"readOnly\": true\n        },\n        \"recipient_count\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Count of the recipients on the associated list.\",\n          \"readOnly\": true\n        },\n        \"segment_opts\": {\n          \"type\": \"object\",\n          \"description\": \"Segmentation options for targeting a subset of the list.\",\n          \"properties\": {\n            \"saved_segment_id\": {\n              \"type\": \"integer\",\n              \"description\": \"The ID for an existing saved segment.\"\n            },\n            \"prebuilt_segment_id\": {\n              \"type\": \"string\",\n              \"description\": \"The prebuilt segment ID, if a prebuilt segment has been designated.\"\n            },\n            \"match\": {\n              \"type\": \"string\",\n              \"description\": \"Segment match type.\",\n              \"enum\": [\"any\", \"all\"]\n            },\n            \"conditions\": {\n              \"type\": \"array\",\n              \"description\": \"An array of segment\
  \ condition objects.\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"condition_type\": {\n                    \"type\": \"string\",\n                    \"description\": \"The type of segment condition.\"\n                  },\n                  \"field\": {\n                    \"type\": \"string\",\n                    \"description\": \"The field to segment on.\"\n                  },\n                  \"op\": {\n                    \"type\": \"string\",\n                    \"description\": \"The operator for the condition.\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"description\": \"The value to compare against.\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"The settings for the campaign,\
  \ including subject line, from name, and reply-to address.\",\n      \"properties\": {\n        \"subject_line\": {\n          \"type\": \"string\",\n          \"description\": \"The subject line for the campaign.\"\n        },\n        \"preview_text\": {\n          \"type\": \"string\",\n          \"description\": \"The preview text for the campaign, shown in email client inboxes.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The title of the campaign.\"\n        },\n        \"from_name\": {\n          \"type\": \"string\",\n          \"description\": \"The 'from' name on the campaign (not an email address).\"\n        },\n        \"reply_to\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The reply-to email address for the campaign.\"\n        },\n        \"use_conversation\": {\n          \"type\": \"boolean\",\n          \"description\": \"Use Mailchimp Conversation feature to\
  \ manage out-of-office replies.\"\n        },\n        \"to_name\": {\n          \"type\": \"string\",\n          \"description\": \"The campaign's custom 'To' name. Typically the first name merge field.\"\n        },\n        \"folder_id\": {\n          \"type\": \"string\",\n          \"description\": \"If the campaign is listed in a folder, the ID for that folder.\"\n        },\n        \"authenticate\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether Mailchimp authenticated the campaign. Defaults to true.\"\n        },\n        \"auto_footer\": {\n          \"type\": \"boolean\",\n          \"description\": \"Automatically append Mailchimp's default footer to the campaign.\"\n        },\n        \"inline_css\": {\n          \"type\": \"boolean\",\n          \"description\": \"Automatically inline the CSS included with the campaign content.\"\n        },\n        \"auto_tweet\": {\n          \"type\": \"boolean\",\n          \"description\": \"Automatically\
  \ tweet a link to the campaign archive page when the campaign is sent.\"\n        },\n        \"fb_comments\": {\n          \"type\": \"boolean\",\n          \"description\": \"Allows Facebook comments on the campaign (also determines determine the text of the Facebook post).\"\n        },\n        \"template_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID for the template used in this campaign.\"\n        }\n      }\n    },\n    \"tracking\": {\n      \"type\": \"object\",\n      \"description\": \"The tracking options for a campaign.\",\n      \"properties\": {\n        \"opens\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to track opens. Defaults to true.\"\n        },\n        \"html_clicks\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to track clicks in the HTML version of the campaign. Defaults to true.\"\n        },\n        \"text_clicks\": {\n          \"type\": \"boolean\",\n        \
  \  \"description\": \"Whether to track clicks in the plain-text version of the campaign. Defaults to true.\"\n        },\n        \"goal_tracking\": {\n          \"type\": \"boolean\",\n          \"description\": \"Deprecated.\"\n        },\n        \"ecomm360\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to enable e-commerce tracking.\"\n        },\n        \"google_analytics\": {\n          \"type\": \"string\",\n          \"description\": \"The custom slug for Google Analytics tracking (max 50 bytes).\"\n        },\n        \"clicktale\": {\n          \"type\": \"string\",\n          \"description\": \"Deprecated.\"\n        }\n      }\n    },\n    \"report_summary\": {\n      \"type\": \"object\",\n      \"description\": \"For sent campaigns, a summary of opens, clicks, and e-commerce data.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"opens\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of opens\
  \ for a campaign.\"\n        },\n        \"unique_opens\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of unique opens.\"\n        },\n        \"open_rate\": {\n          \"type\": \"number\",\n          \"description\": \"The number of unique opens divided by the total number of successful deliveries.\"\n        },\n        \"clicks\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of clicks for a campaign.\"\n        },\n        \"subscriber_clicks\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of unique clicks.\"\n        },\n        \"click_rate\": {\n          \"type\": \"number\",\n          \"description\": \"The number of unique clicks divided by the total number of successful deliveries.\"\n        },\n        \"ecommerce\": {\n          \"type\": \"object\",\n          \"description\": \"E-commerce stats for a campaign.\",\n          \"properties\": {\n            \"total_orders\"\
  : {\n              \"type\": \"integer\",\n              \"description\": \"The total orders for a campaign.\"\n            },\n            \"total_spent\": {\n              \"type\": \"number\",\n              \"description\": \"The total spent for a campaign.\"\n            },\n            \"total_revenue\": {\n              \"type\": \"number\",\n              \"description\": \"The total revenue for a campaign.\"\n            }\n          }\n        }\n      }\n    },\n    \"delivery_status\": {\n      \"type\": \"object\",\n      \"description\": \"Updates on campaigns in the process of sending.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether Campaign Delivery Status is enabled for this account and target campaign.\"\n        },\n        \"can_cancel\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether a campaign send can be canceled.\"\n        },\n     \
  \   \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The current state of a campaign delivery.\",\n          \"enum\": [\"delivering\", \"delivered\", \"canceling\", \"canceled\"]\n        },\n        \"emails_sent\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of emails confirmed sent for this campaign so far.\"\n        },\n        \"emails_canceled\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of emails canceled for this campaign.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"type\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/campaign.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: Mailchimp Campaign
---
