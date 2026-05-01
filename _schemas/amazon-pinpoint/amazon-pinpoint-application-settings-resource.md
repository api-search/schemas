---
description: Provides information about an application, including the default settings for an application.
layout: schema
name: ApplicationSettingsResource
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: CampaignHook
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Limits
  type: object
- description: ''
  name: QuietTime
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-application-settings-resource-schema.json
slug: amazon-pinpoint-application-settings-resource
source_filename: amazon-pinpoint-application-settings-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-application-settings-resource-schema.json\",\n  \"title\": \"ApplicationSettingsResource\",\n  \"description\": \"Provides information about an application, including the default settings for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application. This identifier is displayed as the <b>Project ID</b> on the Amazon Pinpoint console.\"\n        }\n      ]\n    },\n    \"CampaignHook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignHook\"\n        },\n        {\n          \"description\": \"The settings for the AWS Lambda function to invoke\
  \ by default as a code hook for campaigns in the application. You can use this hook to customize segments that are used by campaigns in the application.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the application's settings were last modified.\"\n        }\n      ]\n    },\n    \"Limits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignLimits\"\n        },\n        {\n          \"description\": \"The default sending limits for campaigns in the application.\"\n        }\n      ]\n    },\n    \"QuietTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuietTime\"\n        },\n        {\n          \"description\": \"<p>The default quiet time for campaigns in the application. Quiet time is a specific time range when messages aren't\
  \ sent to endpoints, if all the following conditions are met:</p> <ul><li><p>The EndpointDemographic.Timezone property of the endpoint is set to a valid value.</p></li> <li><p>The current time in the endpoint's time zone is later than or equal to the time specified by the QuietTime.Start property for the application (or a campaign or journey that has custom quiet time settings).</p></li> <li><p>The current time in the endpoint's time zone is earlier than or equal to the time specified by the QuietTime.End property for the application (or a campaign or journey that has custom quiet time settings).</p></li></ul> <p>If any of the preceding conditions isn't met, the endpoint will receive messages from a campaign or journey, even if quiet time is enabled.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-application-settings-resource-schema.json
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
title: ApplicationSettingsResource
---
