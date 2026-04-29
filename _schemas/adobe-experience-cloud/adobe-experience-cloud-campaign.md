---
description: A marketing campaign entity representing a coordinated marketing effort across channels such as email, SMS, push, and in-app, used in both Adobe Campaign and Journey Optimizer for audience targeting and message delivery.
layout: schema
name: Adobe Experience Cloud Campaign
properties_list:
- description: The unique identifier for the campaign.
  name: campaignId
  type: string
- description: The human-readable name of the campaign.
  name: name
  type: string
- description: A description of the campaign purpose and goals.
  name: description
  type: string
- description: The primary delivery channel.
  name: channel
  type: string
- description: The current status of the campaign.
  name: status
  type: string
- description: The target audience for the campaign.
  name: audience
  type: object
- description: The message content configuration.
  name: content
  type: object
- description: The campaign delivery schedule.
  name: schedule
  type: object
- description: Campaign performance metrics.
  name: metrics
  type: object
- description: When the campaign was created.
  name: created
  type: string
- description: When the campaign was last modified.
  name: lastModified
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/adobe-experience-cloud-campaign.json
slug: adobe-experience-cloud-campaign
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"adobe-experience-cloud-campaign.json\",\n  \"title\": \"Adobe Experience Cloud Campaign\",\n  \"description\": \"A marketing campaign entity representing a coordinated marketing effort across channels such as email, SMS, push, and in-app, used in both Adobe Campaign and Journey Optimizer for audience targeting and message delivery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the campaign.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the campaign.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the campaign purpose and goals.\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"enum\": [\"email\", \"sms\", \"push\", \"inApp\", \"directMail\"],\n      \"\
  description\": \"The primary delivery channel.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"scheduled\", \"live\", \"paused\", \"completed\", \"cancelled\"],\n      \"description\": \"The current status of the campaign.\"\n    },\n    \"audience\": {\n      \"type\": \"object\",\n      \"description\": \"The target audience for the campaign.\",\n      \"properties\": {\n        \"segmentId\": {\n          \"type\": \"string\",\n          \"description\": \"The segment defining the target audience.\"\n        },\n        \"estimatedSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Estimated number of profiles in the target audience.\"\n        }\n      }\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"description\": \"The message content configuration.\",\n      \"properties\": {\n        \"subject\": {\n          \"type\": \"string\",\n          \"description\": \"The message subject line (for email).\"\
  \n        },\n        \"body\": {\n          \"type\": \"string\",\n          \"description\": \"The message body content.\"\n        },\n        \"templateId\": {\n          \"type\": \"string\",\n          \"description\": \"Reference to a content template.\"\n        },\n        \"sender\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"format\": \"email\"\n            }\n          }\n        }\n      }\n    },\n    \"schedule\": {\n      \"type\": \"object\",\n      \"description\": \"The campaign delivery schedule.\",\n      \"properties\": {\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the campaign delivery begins.\"\n        },\n        \"endDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n\
  \          \"description\": \"When the campaign delivery ends.\"\n        },\n        \"timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The timezone for schedule evaluation.\"\n        },\n        \"recurring\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a recurring campaign.\"\n        }\n      }\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Campaign performance metrics.\",\n      \"properties\": {\n        \"sent\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of messages sent.\"\n        },\n        \"delivered\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of messages delivered.\"\n        },\n        \"opened\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of messages opened.\"\n        },\n        \"clicked\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of link clicks.\"\
  \n        },\n        \"bounced\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of bounced messages.\"\n        },\n        \"unsubscribed\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of unsubscribes.\"\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the campaign was created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the campaign was last modified.\"\n    }\n  },\n  \"required\": [\"campaignId\", \"name\", \"channel\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/adobe-experience-cloud-campaign.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Adobe Experience Cloud Campaign
---
