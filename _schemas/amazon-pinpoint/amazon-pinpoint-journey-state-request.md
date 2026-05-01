---
description: Changes the status of a journey.
layout: schema
name: JourneyStateRequest
properties_list:
- description: ''
  name: State
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-journey-state-request-schema.json
slug: amazon-pinpoint-journey-state-request
source_filename: amazon-pinpoint-journey-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-state-request-schema.json\",\n  \"title\": \"JourneyStateRequest\",\n  \"description\": \"Changes the status of a journey.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/State\"\n        },\n        {\n          \"description\": \"<p>The status of the journey. Currently, Supported values are ACTIVE, PAUSED, and CANCELLED</p> <p>If you cancel a journey, Amazon Pinpoint continues to perform activities that are currently in progress, until those activities are complete. Amazon Pinpoint also continues to collect and aggregate analytics data for those activities, until they are complete, and any activities that were complete when you cancelled the journey.</p> <p>After you cancel a journey,\
  \ you can't add, change, or remove any activities from the journey. In addition, Amazon Pinpoint stops evaluating the journey and doesn't perform any activities that haven't started.</p> <p>When the journey is paused, Amazon Pinpoint continues to perform activities that are currently in progress, until those activities are complete. Endpoints will stop entering journeys when the journey is paused and will resume entering the journey after the journey is resumed. For wait activities, wait time is paused when the journey is paused. Currently, PAUSED only supports journeys with a segment refresh interval.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-journey-state-request-schema.json
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
title: JourneyStateRequest
---
