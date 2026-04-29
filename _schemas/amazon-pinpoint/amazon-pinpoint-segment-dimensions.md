---
description: Specifies the dimension settings for a segment.
layout: schema
name: SegmentDimensions
properties_list:
- description: ''
  name: Attributes
  type: object
- description: ''
  name: Behavior
  type: object
- description: ''
  name: Demographic
  type: object
- description: ''
  name: Location
  type: object
- description: ''
  name: Metrics
  type: object
- description: ''
  name: UserAttributes
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-dimensions-schema.json
slug: amazon-pinpoint-segment-dimensions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-dimensions-schema.json\",\n  \"title\": \"SegmentDimensions\",\n  \"description\": \"Specifies the dimension settings for a segment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfAttributeDimension\"\n        },\n        {\n          \"description\": \"One or more custom attributes to use as criteria for the segment.\"\n        }\n      ]\n    },\n    \"Behavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentBehaviors\"\n        },\n        {\n          \"description\": \"The behavior-based criteria, such as how recently users have used your app, for the segment.\"\n        }\n      ]\n    },\n    \"Demographic\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/SegmentDemographics\"\n        },\n        {\n          \"description\": \"The demographic-based criteria, such as device platform, for the segment.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentLocation\"\n        },\n        {\n          \"description\": \"The location-based criteria, such as region or GPS coordinates, for the segment.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfMetricDimension\"\n        },\n        {\n          \"description\": \"One or more custom metrics to use as criteria for the segment.\"\n        }\n      ]\n    },\n    \"UserAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfAttributeDimension\"\n        },\n        {\n          \"description\": \"One or more custom user attributes to use as\
  \ criteria for the segment.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-dimensions-schema.json
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
title: SegmentDimensions
---
