---
description: Provides information about the status and settings of the email channel for an application.
layout: schema
name: EmailChannelResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: ConfigurationSet
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: FromAddress
  type: object
- description: ''
  name: HasCredential
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Identity
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
  name: MessagesPerSecond
  type: object
- description: ''
  name: Platform
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Version
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-email-channel-response-schema.json
slug: amazon-pinpoint-email-channel-response
source_filename: amazon-pinpoint-email-channel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-email-channel-response-schema.json\",\n  \"title\": \"EmailChannelResponse\",\n  \"description\": \"Provides information about the status and settings of the email channel for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that the email channel applies to.\"\n        }\n      ]\n    },\n    \"ConfigurationSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/ses/latest/APIReference/API_ConfigurationSet.html\\\">Amazon SES configuration\
  \ set</a> that's applied to messages that are sent through the channel.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the email channel was enabled.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the email channel is enabled for the application.\"\n        }\n      ]\n    },\n    \"FromAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The verified email address that email is sent from when you send email through the channel.\"\n        }\n      ]\n    },\n    \"HasCredential\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\
  \n        },\n        {\n          \"description\": \"(Not used) This property is retained only for backward compatibility.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"(Deprecated) An identifier for the email channel. This property is retained only for backward compatibility.\"\n        }\n      ]\n    },\n    \"Identity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \" <p>The Amazon Resource Name (ARN) of the identity, verified with Amazon Simple Email Service (Amazon SES), that's used when you send email through the channel.</p>\"\n        }\n      ]\n    },\n    \"IsArchived\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the email channel\
  \ is archived.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The user who last modified the email channel.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the email channel was last modified.\"\n        }\n      ]\n    },\n    \"MessagesPerSecond\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The maximum number of emails that can be sent through the channel each second.\"\n        }\n      ]\n    },\n    \"Platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\"\
  : \"The type of messaging or notification platform for the channel. For the email channel, this value is EMAIL.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \" <p>The ARN of the AWS Identity and Access Management (IAM) role that Amazon Pinpoint uses to submit email-related event data for the channel.</p>\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The current version of the email channel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Platform\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-email-channel-response-schema.json
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
title: EmailChannelResponse
---
