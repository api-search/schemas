---
description: Specifies the base segments and dimensions for a segment, and the relationships between these base segments and dimensions.
layout: schema
name: SegmentGroup
properties_list:
- description: ''
  name: Dimensions
  type: object
- description: ''
  name: SourceSegments
  type: object
- description: ''
  name: SourceType
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-group-schema.json
slug: amazon-pinpoint-segment-group
source_filename: amazon-pinpoint-segment-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-group-schema.json\",\n  \"title\": \"SegmentGroup\",\n  \"description\": \"Specifies the base segments and dimensions for a segment, and the relationships between these base segments and dimensions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Dimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfSegmentDimensions\"\n        },\n        {\n          \"description\": \"An array that defines the dimensions for the segment.\"\n        }\n      ]\n    },\n    \"SourceSegments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfSegmentReference\"\n        },\n        {\n          \"description\": \"<p>The base segment to build the segment on. A base segment, also referred to as a <i>source segment</i>,\
  \ defines the initial population of endpoints for a segment. When you add dimensions to a segment, Amazon Pinpoint filters the base segment by using the dimensions that you specify.</p> <p>You can specify more than one dimensional segment or only one imported segment. If you specify an imported segment, the Amazon Pinpoint console displays a segment size estimate that indicates the size of the imported segment without any filters applied to it.</p>\"\n        }\n      ]\n    },\n    \"SourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceType\"\n        },\n        {\n          \"description\": \"Specifies how to handle multiple base segments for the segment. For example, if you specify three base segments for the segment, whether the resulting segment is based on all, any, or none of the base segments.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n\
  \        {\n          \"description\": \"Specifies how to handle multiple dimensions for the segment. For example, if you specify three dimensions for the segment, whether the resulting segment includes endpoints that match all, any, or none of the dimensions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-group-schema.json
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
title: SegmentGroup
---
