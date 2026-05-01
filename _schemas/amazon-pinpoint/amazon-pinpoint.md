---
description: Schema defining the structure of an Amazon Pinpoint application resource, including campaigns, segments, channels, and messaging configuration for multi-channel marketing communications.
layout: schema
name: Amazon Pinpoint Application Definition
properties_list:
- description: The unique identifier for the application.
  name: Id
  type: string
- description: The Amazon Resource Name of the application.
  name: Arn
  type: string
- description: The display name of the application.
  name: Name
  type: string
- description: Tags associated with the application.
  name: tags
  type: object
- description: The date and time when the application was created.
  name: CreationDate
  type: string
- description: The campaigns for the application.
  name: Campaigns
  type: array
- description: The audience segments for the application.
  name: Segments
  type: array
- description: ''
  name: Channels
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-schema.json
slug: amazon-pinpoint
source_filename: amazon-pinpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-pinpoint/application-definition\",\n  \"title\": \"Amazon Pinpoint Application Definition\",\n  \"description\": \"Schema defining the structure of an Amazon Pinpoint application resource, including campaigns, segments, channels, and messaging configuration for multi-channel marketing communications.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\"\n  ],\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the application.\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name of the application.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the application.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\
  \n      },\n      \"description\": \"Tags associated with the application.\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the application was created.\"\n    },\n    \"Campaigns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Campaign\"\n      },\n      \"description\": \"The campaigns for the application.\"\n    },\n    \"Segments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Segment\"\n      },\n      \"description\": \"The audience segments for the application.\"\n    },\n    \"Channels\": {\n      \"$ref\": \"#/$defs/Channels\"\n    }\n  },\n  \"$defs\": {\n    \"Campaign\": {\n      \"type\": \"object\",\n      \"description\": \"A messaging campaign that engages a targeted audience segment.\",\n      \"required\": [\n        \"Name\"\n      ],\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The unique identifier of the campaign.\"\n        },\n        \"ApplicationId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the application.\"\n        },\n        \"Arn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the campaign.\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the campaign.\"\n        },\n        \"Description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the campaign.\"\n        },\n        \"SegmentId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the target segment.\"\n        },\n        \"SegmentVersion\": {\n          \"type\": \"integer\",\n          \"description\": \"The version of the target segment.\"\n        },\n        \"State\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"CampaignStatus\": {\n\
  \              \"type\": \"string\",\n              \"enum\": [\n                \"SCHEDULED\",\n                \"EXECUTING\",\n                \"PENDING_NEXT_RUN\",\n                \"COMPLETED\",\n                \"PAUSED\",\n                \"DELETED\",\n                \"INVALID\"\n              ]\n            }\n          }\n        },\n        \"Schedule\": {\n          \"$ref\": \"#/$defs/Schedule\"\n        },\n        \"MessageConfiguration\": {\n          \"$ref\": \"#/$defs/MessageConfiguration\"\n        },\n        \"IsPaused\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the campaign is paused.\"\n        },\n        \"CreationDate\": {\n          \"type\": \"string\"\n        },\n        \"LastModifiedDate\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Segment\": {\n      \"type\": \"object\",\n      \"description\": \"An audience segment that defines a group of users for targeting.\",\n      \"properties\": {\n   \
  \     \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the segment.\"\n        },\n        \"ApplicationId\": {\n          \"type\": \"string\"\n        },\n        \"Arn\": {\n          \"type\": \"string\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the segment.\"\n        },\n        \"SegmentType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"DIMENSIONAL\",\n            \"IMPORT\"\n          ],\n          \"description\": \"The segment type.\"\n        },\n        \"Dimensions\": {\n          \"$ref\": \"#/$defs/SegmentDimensions\"\n        },\n        \"CreationDate\": {\n          \"type\": \"string\"\n        },\n        \"LastModifiedDate\": {\n          \"type\": \"string\"\n        },\n        \"Version\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"Schedule\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"The schedule settings for a campaign.\",\n      \"properties\": {\n        \"StartTime\": {\n          \"type\": \"string\",\n          \"description\": \"The scheduled time when the campaign begins.\"\n        },\n        \"EndTime\": {\n          \"type\": \"string\",\n          \"description\": \"The scheduled time when the campaign ends.\"\n        },\n        \"Frequency\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ONCE\",\n            \"HOURLY\",\n            \"DAILY\",\n            \"WEEKLY\",\n            \"MONTHLY\",\n            \"EVENT\",\n            \"IN_APP_EVENT\"\n          ],\n          \"description\": \"How often the campaign is sent.\"\n        },\n        \"IsLocalTime\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to use local time for the schedule.\"\n        },\n        \"Timezone\": {\n          \"type\": \"string\",\n          \"description\": \"The starting UTC offset for the campaign schedule.\"\
  \n        }\n      }\n    },\n    \"MessageConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"The message configuration for a campaign.\",\n      \"properties\": {\n        \"EmailMessage\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Title\": { \"type\": \"string\" },\n            \"Body\": { \"type\": \"string\" },\n            \"HtmlBody\": { \"type\": \"string\" },\n            \"FromAddress\": { \"type\": \"string\" }\n          }\n        },\n        \"SMSMessage\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Body\": { \"type\": \"string\" },\n            \"MessageType\": {\n              \"type\": \"string\",\n              \"enum\": [\"TRANSACTIONAL\", \"PROMOTIONAL\"]\n            },\n            \"SenderId\": { \"type\": \"string\" }\n          }\n        },\n        \"GCMMessage\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Title\": { \"type\": \"\
  string\" },\n            \"Body\": { \"type\": \"string\" },\n            \"Action\": {\n              \"type\": \"string\",\n              \"enum\": [\"OPEN_APP\", \"DEEP_LINK\", \"URL\"]\n            }\n          }\n        },\n        \"APNSMessage\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Title\": { \"type\": \"string\" },\n            \"Body\": { \"type\": \"string\" },\n            \"Action\": {\n              \"type\": \"string\",\n              \"enum\": [\"OPEN_APP\", \"DEEP_LINK\", \"URL\"]\n            }\n          }\n        }\n      }\n    },\n    \"SegmentDimensions\": {\n      \"type\": \"object\",\n      \"description\": \"The dimension settings for a segment.\",\n      \"properties\": {\n        \"Demographic\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"AppVersion\": { \"type\": \"object\" },\n            \"Channel\": { \"type\": \"object\" },\n            \"DeviceType\": { \"type\": \"object\"\
  \ },\n            \"Make\": { \"type\": \"object\" },\n            \"Model\": { \"type\": \"object\" },\n            \"Platform\": { \"type\": \"object\" }\n          }\n        },\n        \"Location\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Country\": { \"type\": \"object\" },\n            \"GPSPoint\": { \"type\": \"object\" }\n          }\n        }\n      }\n    },\n    \"Channels\": {\n      \"type\": \"object\",\n      \"description\": \"The messaging channel configurations for the application.\",\n      \"properties\": {\n        \"Email\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Enabled\": { \"type\": \"boolean\" },\n            \"FromAddress\": { \"type\": \"string\" },\n            \"Identity\": { \"type\": \"string\" }\n          }\n        },\n        \"SMS\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Enabled\": { \"type\": \"boolean\" },\n            \"SenderId\"\
  : { \"type\": \"string\" },\n            \"ShortCode\": { \"type\": \"string\" }\n          }\n        },\n        \"Push\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"APNs\": { \"type\": \"object\" },\n            \"GCM\": { \"type\": \"object\" }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-schema.json
tags:
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
title: Amazon Pinpoint Application Definition
---
