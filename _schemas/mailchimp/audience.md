---
description: A Mailchimp audience (also known as a list). Audiences contain subscribers who have opted in to receive correspondence from you or your organization. They hold contact information, segmentation data, campaign defaults, and compliance settings.
layout: schema
name: Mailchimp Audience (List)
properties_list:
- description: A string that uniquely identifies this list.
  name: id
  type: string
- description: The ID used in the Mailchimp web application.
  name: web_id
  type: integer
- description: The name of the list/audience.
  name: name
  type: string
- description: Contact information displayed in campaign footers to comply with international spam laws.
  name: contact
  type: object
- description: The permission reminder for the list, reminding subscribers how they signed up.
  name: permission_reminder
  type: string
- description: Whether campaigns for this list use the Archive Bar in archives by default.
  name: use_archive_bar
  type: boolean
- description: Default values for campaigns created for this list.
  name: campaign_defaults
  type: object
- description: The email address to send subscribe notifications to. Set to empty string to disable.
  name: notify_on_subscribe
  type: string
- description: The email address to send unsubscribe notifications to. Set to empty string to disable.
  name: notify_on_unsubscribe
  type: string
- description: The date and time that this list was created in ISO 8601 format.
  name: date_created
  type: string
- description: An auto-generated activity score for the list (0-5).
  name: list_rating
  type: integer
- description: Whether the list supports multiple email formats (HTML and plain-text). When true, subscribers can choose their preferred format.
  name: email_type_option
  type: boolean
- description: The URL-shortened version of this list's subscribe form.
  name: subscribe_url_short
  type: string
- description: The full version of this list's subscribe form URL.
  name: subscribe_url_long
  type: string
- description: The list's Email Beamer address for creating campaigns via email.
  name: beamer_address
  type: string
- description: Legacy visibility setting. No longer used.
  name: visibility
  type: string
- description: Whether to require the subscriber to confirm subscription via email.
  name: double_optin
  type: boolean
- description: Whether this list has a welcome automation connected.
  name: has_welcome
  type: boolean
- description: Whether the list has marketing permissions (GDPR) enabled.
  name: marketing_permissions
  type: boolean
- description: Any list-specific modules installed for this list.
  name: modules
  type: array
- description: Stats for the list, including subscriber counts and campaign performance.
  name: stats
  type: object
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/audience.json
slug: audience
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/messaging/mailchimp/json-schema/audience.json\",\n  \"title\": \"Mailchimp Audience (List)\",\n  \"description\": \"A Mailchimp audience (also known as a list). Audiences contain subscribers who have opted in to receive correspondence from you or your organization. They hold contact information, segmentation data, campaign defaults, and compliance settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A string that uniquely identifies this list.\",\n      \"readOnly\": true\n    },\n    \"web_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID used in the Mailchimp web application.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the list/audience.\"\n    },\n    \"contact\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Contact information displayed in campaign footers to comply with international spam laws.\",\n      \"properties\": {\n        \"company\": {\n          \"type\": \"string\",\n          \"description\": \"The company name for the list.\"\n        },\n        \"address1\": {\n          \"type\": \"string\",\n          \"description\": \"The street address for the list contact.\"\n        },\n        \"address2\": {\n          \"type\": \"string\",\n          \"description\": \"The second line of the street address.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city for the list contact.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The state for the list contact.\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"description\": \"The postal or zip code for the list contact.\"\n        },\n        \"country\": {\n          \"\
  type\": \"string\",\n          \"description\": \"A two-character ISO 3166 country code. Defaults to US if invalid.\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"The phone number for the list contact.\"\n        }\n      },\n      \"required\": [\"company\", \"address1\", \"city\", \"state\", \"zip\", \"country\"]\n    },\n    \"permission_reminder\": {\n      \"type\": \"string\",\n      \"description\": \"The permission reminder for the list, reminding subscribers how they signed up.\"\n    },\n    \"use_archive_bar\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether campaigns for this list use the Archive Bar in archives by default.\",\n      \"default\": false\n    },\n    \"campaign_defaults\": {\n      \"type\": \"object\",\n      \"description\": \"Default values for campaigns created for this list.\",\n      \"properties\": {\n        \"from_name\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The default from name for campaigns sent to this list.\"\n        },\n        \"from_email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The default from email for campaigns sent to this list.\"\n        },\n        \"subject\": {\n          \"type\": \"string\",\n          \"description\": \"The default subject line for campaigns sent to this list.\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"The default language for this list's forms.\"\n        }\n      },\n      \"required\": [\"from_name\", \"from_email\", \"subject\", \"language\"]\n    },\n    \"notify_on_subscribe\": {\n      \"type\": \"string\",\n      \"description\": \"The email address to send subscribe notifications to. Set to empty string to disable.\"\n    },\n    \"notify_on_unsubscribe\": {\n      \"type\": \"string\",\n      \"description\": \"The email address to\
  \ send unsubscribe notifications to. Set to empty string to disable.\"\n    },\n    \"date_created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that this list was created in ISO 8601 format.\",\n      \"readOnly\": true\n    },\n    \"list_rating\": {\n      \"type\": \"integer\",\n      \"description\": \"An auto-generated activity score for the list (0-5).\",\n      \"minimum\": 0,\n      \"maximum\": 5,\n      \"readOnly\": true\n    },\n    \"email_type_option\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the list supports multiple email formats (HTML and plain-text). When true, subscribers can choose their preferred format.\"\n    },\n    \"subscribe_url_short\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL-shortened version of this list's subscribe form.\",\n      \"readOnly\": true\n    },\n    \"subscribe_url_long\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"uri\",\n      \"description\": \"The full version of this list's subscribe form URL.\",\n      \"readOnly\": true\n    },\n    \"beamer_address\": {\n      \"type\": \"string\",\n      \"description\": \"The list's Email Beamer address for creating campaigns via email.\",\n      \"readOnly\": true\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Legacy visibility setting. No longer used.\",\n      \"enum\": [\"pub\", \"prv\"]\n    },\n    \"double_optin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to require the subscriber to confirm subscription via email.\",\n      \"default\": false\n    },\n    \"has_welcome\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this list has a welcome automation connected.\",\n      \"default\": false\n    },\n    \"marketing_permissions\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the list has marketing permissions (GDPR) enabled.\"\
  ,\n      \"default\": false\n    },\n    \"modules\": {\n      \"type\": \"array\",\n      \"description\": \"Any list-specific modules installed for this list.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true\n    },\n    \"stats\": {\n      \"type\": \"object\",\n      \"description\": \"Stats for the list, including subscriber counts and campaign performance.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"member_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of active members in the list.\"\n        },\n        \"total_contacts\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of contacts in the list, including subscribed, unsubscribed, pending, cleaned, and transactional contacts.\"\n        },\n        \"unsubscribe_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of members who have unsubscribed from the list.\"\n   \
  \     },\n        \"cleaned_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of members cleaned from the list (hard bounced).\"\n        },\n        \"member_count_since_send\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of active members in the list since the last campaign was sent.\"\n        },\n        \"unsubscribe_count_since_send\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of members who have unsubscribed since the last campaign was sent.\"\n        },\n        \"cleaned_count_since_send\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of members cleaned from the list since the last campaign was sent.\"\n        },\n        \"campaign_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of campaigns in any status that use this list.\"\n        },\n        \"campaign_last_sent\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the last campaign was sent to this list in ISO 8601 format.\"\n        },\n        \"merge_field_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of merge fields for this list (not including EMAIL).\"\n        },\n        \"avg_sub_rate\": {\n          \"type\": \"number\",\n          \"description\": \"The average number of subscriptions per month for the list.\"\n        },\n        \"avg_unsub_rate\": {\n          \"type\": \"number\",\n          \"description\": \"The average number of unsubscriptions per month for the list.\"\n        },\n        \"target_sub_rate\": {\n          \"type\": \"number\",\n          \"description\": \"The target number of subscriptions per month for the list to keep it growing.\"\n        },\n        \"open_rate\": {\n          \"type\": \"number\",\n          \"description\": \"The average open rate (a percentage represented as\
  \ a number between 0 and 100) per campaign for the list.\"\n        },\n        \"click_rate\": {\n          \"type\": \"number\",\n          \"description\": \"The average click rate (a percentage represented as a number between 0 and 100) per campaign for the list.\"\n        },\n        \"last_sub_date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time of the last subscribe in ISO 8601 format.\"\n        },\n        \"last_unsub_date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time of the last unsubscribe in ISO 8601 format.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"contact\", \"permission_reminder\", \"campaign_defaults\", \"email_type_option\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/audience.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: Mailchimp Audience (List)
---
