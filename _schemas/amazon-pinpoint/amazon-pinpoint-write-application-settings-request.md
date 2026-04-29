---
description: Specifies the default settings for an application.
layout: schema
name: WriteApplicationSettingsRequest
properties_list:
- description: ''
  name: CampaignHook
  type: object
- description: ''
  name: CloudWatchMetricsEnabled
  type: object
- description: ''
  name: EventTaggingEnabled
  type: object
- description: ''
  name: Limits
  type: object
- description: ''
  name: QuietTime
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-write-application-settings-request-schema.json
slug: amazon-pinpoint-write-application-settings-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-write-application-settings-request-schema.json\",\n  \"title\": \"WriteApplicationSettingsRequest\",\n  \"description\": \"Specifies the default settings for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CampaignHook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignHook\"\n        },\n        {\n          \"description\": \"<p>The settings for the AWS Lambda function to invoke by default as a code hook for campaigns in the application. You can use this hook to customize segments that are used by campaigns in the application.</p> <p>To override these settings and define custom settings for a specific campaign, use the CampaignHook object of the <link linkend=\\\"apps-application-id-campaigns-campaign-id\\\">Campaign</link>\
  \ resource.</p>\"\n        }\n      ]\n    },\n    \"CloudWatchMetricsEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to enable application-related alarms in Amazon CloudWatch.\"\n        }\n      ]\n    },\n    \"EventTaggingEnabled\": {\n      \"$ref\": \"#/components/schemas/__boolean\"\n    },\n    \"Limits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignLimits\"\n        },\n        {\n          \"description\": \"The default sending limits for campaigns in the application. To override these limits and define custom limits for a specific campaign or journey, use the <link linkend=\\\"apps-application-id-campaigns-campaign-id\\\">Campaign</link> resource or the <link  linkend=\\\"apps-application-id-journeys-journey-id\\\">Journey</link> resource, respectively.\"\n        }\n      ]\n    },\n    \"QuietTime\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuietTime\"\n        },\n        {\n          \"description\": \"<p>The default quiet time for campaigns in the application. Quiet time is a specific time range when messages aren't sent to endpoints, if all the following conditions are met:</p> <ul><li><p>The EndpointDemographic.Timezone property of the endpoint is set to a valid value.</p></li> <li><p>The current time in the endpoint's time zone is later than or equal to the time specified by the QuietTime.Start property for the application (or a campaign or journey that has custom quiet time settings).</p></li> <li><p>The current time in the endpoint's time zone is earlier than or equal to the time specified by the QuietTime.End property for the application (or a campaign or journey that has custom quiet time settings).</p></li></ul> <p>If any of the preceding conditions isn't met, the endpoint will receive messages from a campaign or journey, even if quiet time is enabled.</p>\
  \ <p>To override the default quiet time settings for a specific campaign or journey, use the <link  linkend=\\\"apps-application-id-campaigns-campaign-id\\\">Campaign</link> resource or the <link linkend=\\\"apps-application-id-journeys-journey-id\\\">Journey</link> resource to define a custom quiet time for the campaign or journey.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-write-application-settings-request-schema.json
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
title: WriteApplicationSettingsRequest
---
