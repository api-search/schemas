---
description: Provides information about the status and settings of the SMS channel for an application.
layout: schema
name: SMSChannelResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: HasCredential
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: IsArchived
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Platform
  type: object
- description: ''
  name: PromotionalMessagesPerSecond
  type: object
- description: ''
  name: SenderId
  type: object
- description: ''
  name: ShortCode
  type: object
- description: ''
  name: TransactionalMessagesPerSecond
  type: object
- description: ''
  name: Version
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-sms-channel-response-schema.json
slug: amazon-pinpoint-sms-channel-response
source_filename: amazon-pinpoint-sms-channel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-channel-response-schema.json\",\n  \"title\": \"SMSChannelResponse\",\n  \"description\": \"Provides information about the status and settings of the SMS channel for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that the SMS channel applies to.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the SMS channel was enabled.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the SMS channel is enabled for the application.\"\n        }\n      ]\n    },\n    \"HasCredential\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"(Not used) This property is retained only for backward compatibility.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"(Deprecated) An identifier for the SMS channel. This property is retained only for backward compatibility.\"\n        }\n      ]\n    },\n    \"IsArchived\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the SMS channel is archived.\"\
  \n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The user who last modified the SMS channel.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the SMS channel was last modified.\"\n        }\n      ]\n    },\n    \"Platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The type of messaging or notification platform for the channel. For the SMS channel, this value is SMS.\"\n        }\n      ]\n    },\n    \"PromotionalMessagesPerSecond\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n       \
  \   \"description\": \"The maximum number of promotional messages that you can send through the SMS channel each second.\"\n        }\n      ]\n    },\n    \"SenderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The identity that displays on recipients' devices when they receive messages from the SMS channel.\"\n        }\n      ]\n    },\n    \"ShortCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The registered short code to use when you send messages through the SMS channel.\"\n        }\n      ]\n    },\n    \"TransactionalMessagesPerSecond\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of transactional messages that you can send through the SMS channel each second.\"\n \
  \       }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The current version of the SMS channel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Platform\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-channel-response-schema.json
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
title: SMSChannelResponse
---
