---
description: Specifies the settings that define the relationships between segment groups for a segment.
layout: schema
name: SegmentGroupList
properties_list:
- description: ''
  name: Groups
  type: object
- description: ''
  name: Include
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-group-list-schema.json
slug: amazon-pinpoint-segment-group-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-group-list-schema.json\",\n  \"title\": \"SegmentGroupList\",\n  \"description\": \"Specifies the settings that define the relationships between segment groups for a segment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Groups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListOfSegmentGroup\"\n        },\n        {\n          \"description\": \"An array that defines the set of segment criteria to evaluate when handling segment groups for the segment.\"\n        }\n      ]\n    },\n    \"Include\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Include\"\n        },\n        {\n          \"description\": \"Specifies how to handle multiple segment groups for the segment. For example, if the segment includes\
  \ three segment groups, whether the resulting segment includes endpoints that match all, any, or none of the segment groups.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-group-list-schema.json
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
title: SegmentGroupList
---
