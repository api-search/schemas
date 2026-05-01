---
description: <p>Specifies the settings for a yes/no split activity in a journey. This type of activity sends participants down one of two paths in a journey, based on conditions that you specify.</p> <note><p>To create yes/no split activities that send participants down different paths based on push notification events (such as Open or Received events), your mobile app has to specify the User ID and Endpoint ID values. For more information, see <a href="https://docs.aws.amazon.com/pinpoint/latest/developerguide/integrate.html">Integrating Amazon Pinpoint with your application</a> in the <i>Amazon Pinpoint Developer Guide</i>.</p></note>
layout: schema
name: ConditionalSplitActivity
properties_list:
- description: ''
  name: Condition
  type: object
- description: ''
  name: EvaluationWaitTime
  type: object
- description: ''
  name: FalseActivity
  type: object
- description: ''
  name: TrueActivity
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-conditional-split-activity-schema.json
slug: amazon-pinpoint-conditional-split-activity
source_filename: amazon-pinpoint-conditional-split-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-conditional-split-activity-schema.json\",\n  \"title\": \"ConditionalSplitActivity\",\n  \"description\": \"<p>Specifies the settings for a yes/no split activity in a journey. This type of activity sends participants down one of two paths in a journey, based on conditions that you specify.</p> <note><p>To create yes/no split activities that send participants down different paths based on push notification events (such as Open or Received events), your mobile app has to specify the User ID and Endpoint ID values. For more information, see <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/developerguide/integrate.html\\\">Integrating Amazon Pinpoint with your application</a> in the <i>Amazon Pinpoint Developer Guide</i>.</p></note>\",\n  \"type\": \"object\",\n  \"properties\": {\n\
  \    \"Condition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Condition\"\n        },\n        {\n          \"description\": \"The conditions that define the paths for the activity, and the relationship between the conditions.\"\n        }\n      ]\n    },\n    \"EvaluationWaitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WaitTime\"\n        },\n        {\n          \"description\": \"The amount of time to wait before determining whether the conditions are met, or the date and time when Amazon Pinpoint determines whether the conditions are met.\"\n        }\n      ]\n    },\n    \"FalseActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the activity to perform if the conditions aren't met.\"\n        }\n      ]\n    },\n    \"TrueActivity\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the activity to perform if the conditions are met.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-conditional-split-activity-schema.json
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
title: ConditionalSplitActivity
---
