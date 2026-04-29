---
description: Provides information about the configuration, dimension, and other settings for a segment.
layout: schema
name: SegmentResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Dimensions
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: ImportDefinition
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: SegmentGroups
  type: object
- description: ''
  name: SegmentType
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: Version
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-response-schema.json
slug: amazon-pinpoint-segment-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-response-schema.json\",\n  \"title\": \"SegmentResponse\",\n  \"description\": \"Provides information about the configuration, dimension, and other settings for a segment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that the segment is associated with.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the segment.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time when the segment was created.\"\n        }\n      ]\n    },\n    \"Dimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentDimensions\"\n        },\n        {\n          \"description\": \"The dimension settings for the segment.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the segment.\"\n        }\n      ]\n    },\n    \"ImportDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentImportResource\"\n        },\n        {\n          \"description\": \"The settings for the import job that's associated with the segment.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time when the segment was last modified.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the segment.\"\n        }\n      ]\n    },\n    \"SegmentGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentGroupList\"\n        },\n        {\n          \"description\": \"A list of one or more segment groups that apply to the segment. Each segment group consists of zero or more base segments and the dimensions that are applied to those base segments.\"\n        }\n      ]\n    },\n    \"SegmentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentType\"\n        },\n        {\n          \"description\": \"<p>The segment type. Valid values are:</p> <ul><li><p>DIMENSIONAL\
  \ - A dynamic segment, which is a segment that uses selection criteria that you specify and is based on endpoint data that's reported by your app. Dynamic segments can change over time.</p></li> <li><p>IMPORT - A static segment, which is a segment that uses selection criteria that you specify and is based on endpoint definitions that you import from a file. Imported segments are static; they don't change over time.</p></li></ul>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that identifies the tags that are associated with the segment. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The version\
  \ number of the segment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SegmentType\",\n    \"CreationDate\",\n    \"Id\",\n    \"Arn\",\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-response-schema.json
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
title: SegmentResponse
---
