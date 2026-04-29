---
description: Provides information about the status, configuration, and other settings for a campaign.
layout: schema
name: CampaignResponse
properties_list:
- description: ''
  name: AdditionalTreatments
  type: object
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: CustomDeliveryConfiguration
  type: object
- description: ''
  name: DefaultState
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: HoldoutPercent
  type: object
- description: ''
  name: Hook
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: IsPaused
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Limits
  type: object
- description: ''
  name: MessageConfiguration
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Schedule
  type: object
- description: ''
  name: SegmentId
  type: object
- description: ''
  name: SegmentVersion
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: TemplateConfiguration
  type: object
- description: ''
  name: TreatmentDescription
  type: object
- description: ''
  name: TreatmentName
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: Priority
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-campaign-response-schema.json
slug: amazon-pinpoint-campaign-response
source_filename: amazon-pinpoint-campaign-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-response-schema.json\",\n  \"title\": \"CampaignResponse\",\n  \"description\": \"Provides information about the status, configuration, and other settings for a campaign.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdditionalTreatments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfTreatmentResource\"\n        },\n        {\n          \"description\": \"An array of responses, one for each treatment that you defined for the campaign, in addition to the default treatment.\"\n        }\n      ]\n    },\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that the campaign applies\
  \ to.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the campaign.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the campaign was created.\"\n        }\n      ]\n    },\n    \"CustomDeliveryConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomDeliveryConfiguration\"\n        },\n        {\n          \"description\": \"The delivery configuration settings for sending the campaign through a custom channel.\"\n        }\n      ]\n    },\n    \"DefaultState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignState\"\n        },\n        {\n          \"description\"\
  : \"The current status of the campaign's default treatment. This value exists only for campaigns that have more than one treatment.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the campaign.\"\n        }\n      ]\n    },\n    \"HoldoutPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The allocated percentage of users (segment members) who shouldn't receive messages from the campaign.\"\n        }\n      ]\n    },\n    \"Hook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignHook\"\n        },\n        {\n          \"description\": \"The settings for the AWS Lambda function to use as a code hook for the campaign. You can use this hook to customize the segment that's used by the\
  \ campaign.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the campaign.\"\n        }\n      ]\n    },\n    \"IsPaused\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the campaign is paused. A paused campaign doesn't run unless you resume it by changing this value to false.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the campaign was last modified.\"\n        }\n      ]\n    },\n    \"Limits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignLimits\"\n        },\n        {\n          \"description\"\
  : \"The messaging limits for the campaign.\"\n        }\n      ]\n    },\n    \"MessageConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageConfiguration\"\n        },\n        {\n          \"description\": \"The message configuration settings for the campaign.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the campaign.\"\n        }\n      ]\n    },\n    \"Schedule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Schedule\"\n        },\n        {\n          \"description\": \"The schedule settings for the campaign.\"\n        }\n      ]\n    },\n    \"SegmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the segment that's associated with\
  \ the campaign.\"\n        }\n      ]\n    },\n    \"SegmentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The version number of the segment that's associated with the campaign.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignState\"\n        },\n        {\n          \"description\": \"The current status of the campaign.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that identifies the tags that are associated with the campaign. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"TemplateConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateConfiguration\"\
  \n        },\n        {\n          \"description\": \"The message template that\\u2019s used for the campaign.\"\n        }\n      ]\n    },\n    \"TreatmentDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the default treatment for the campaign.\"\n        }\n      ]\n    },\n    \"TreatmentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom name of the default treatment for the campaign, if the campaign has multiple treatments. A <i>treatment</i> is a variation of a campaign that's used for A/B testing.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The version number of the campaign.\"\n        }\n      ]\n\
  \    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"Defines the priority of the campaign, used to decide the order of messages displayed to user if there are multiple messages scheduled to be displayed at the same moment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LastModifiedDate\",\n    \"CreationDate\",\n    \"SegmentId\",\n    \"SegmentVersion\",\n    \"Id\",\n    \"Arn\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-campaign-response-schema.json
tags:
- AWS
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: CampaignResponse
---
