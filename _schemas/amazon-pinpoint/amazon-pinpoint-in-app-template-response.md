---
description: In-App Template Response.
layout: schema
name: InAppTemplateResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Content
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: CustomConfig
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Layout
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: TemplateDescription
  type: object
- description: ''
  name: TemplateName
  type: object
- description: ''
  name: TemplateType
  type: object
- description: ''
  name: Version
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-in-app-template-response-schema.json
slug: amazon-pinpoint-in-app-template-response
source_filename: amazon-pinpoint-in-app-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-template-response-schema.json\",\n  \"title\": \"InAppTemplateResponse\",\n  \"description\": \"In-App Template Response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The resource arn of the template.\"\n        }\n      ]\n    },\n    \"Content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfInAppMessageContent\"\n        },\n        {\n          \"description\": \"The content of the message, can include up to 5 modals. Each modal must contain a message, a header, and background color. ImageUrl and buttons are optional.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The creation date of the template.\"\n        }\n      ]\n    },\n    \"CustomConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"Custom config to be sent to client.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The last modified date of the template.\"\n        }\n      ]\n    },\n    \"Layout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Layout\"\n        },\n        {\n          \"description\": \"The layout of the message.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n    \
  \    {\n          \"description\": \"A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"TemplateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The description of the template.\"\n        }\n      ]\n    },\n    \"TemplateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the template.\"\n        }\n      ]\n    },\n    \"TemplateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The type of the template.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The version id of the template.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LastModifiedDate\",\n    \"CreationDate\",\n    \"TemplateName\",\n    \"TemplateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-in-app-template-response-schema.json
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
title: InAppTemplateResponse
---
