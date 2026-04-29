---
description: <p>Specifies the settings for a multivariate split activity in a journey. This type of activity sends participants down one of as many as five paths (including a default <i>Else</i> path) in a journey, based on conditions that you specify.</p> <note><p>To create multivariate split activities that send participants down different paths based on push notification events (such as Open or Received events), your mobile app has to specify the User ID and Endpoint ID values. For more information, see <a href="https://docs.aws.amazon.com/pinpoint/latest/developerguide/integrate.html">Integrating Amazon Pinpoint with your application</a> in the <i>Amazon Pinpoint Developer Guide</i>.</p></note>
layout: schema
name: MultiConditionalSplitActivity
properties_list:
- description: ''
  name: Branches
  type: object
- description: ''
  name: DefaultActivity
  type: object
- description: ''
  name: EvaluationWaitTime
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-multi-conditional-split-activity-schema.json
slug: amazon-pinpoint-multi-conditional-split-activity
source_filename: amazon-pinpoint-multi-conditional-split-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-multi-conditional-split-activity-schema.json\",\n  \"title\": \"MultiConditionalSplitActivity\",\n  \"description\": \"<p>Specifies the settings for a multivariate split activity in a journey. This type of activity sends participants down one of as many as five paths (including a default <i>Else</i> path) in a journey, based on conditions that you specify.</p> <note><p>To create multivariate split activities that send participants down different paths based on push notification events (such as Open or Received events), your mobile app has to specify the User ID and Endpoint ID values. For more information, see <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/developerguide/integrate.html\\\">Integrating Amazon Pinpoint with your application</a> in the <i>Amazon Pinpoint Developer\
  \ Guide</i>.</p></note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Branches\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfMultiConditionalBranch\"\n        },\n        {\n          \"description\": \"The paths for the activity, including the conditions for entering each path and the activity to perform for each path.\"\n        }\n      ]\n    },\n    \"DefaultActivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the activity to perform for participants who don't meet any of the conditions specified for other paths in the activity.\"\n        }\n      ]\n    },\n    \"EvaluationWaitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WaitTime\"\n        },\n        {\n          \"description\": \"The amount of time to wait or the date and time when Amazon Pinpoint determines whether\
  \ the conditions are met.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-multi-conditional-split-activity-schema.json
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
title: MultiConditionalSplitActivity
---
