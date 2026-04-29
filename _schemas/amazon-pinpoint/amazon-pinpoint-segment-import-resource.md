---
description: Provides information about the import job that created a segment. An import job is a job that creates a user segment by importing endpoint definitions.
layout: schema
name: SegmentImportResource
properties_list:
- description: ''
  name: ChannelCounts
  type: object
- description: ''
  name: ExternalId
  type: object
- description: ''
  name: Format
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: S3Url
  type: object
- description: ''
  name: Size
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-segment-import-resource-schema.json
slug: amazon-pinpoint-segment-import-resource
source_filename: amazon-pinpoint-segment-import-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-import-resource-schema.json\",\n  \"title\": \"SegmentImportResource\",\n  \"description\": \"Provides information about the import job that created a segment. An import job is a job that creates a user segment by importing endpoint definitions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__integer\"\n        },\n        {\n          \"description\": \"The number of channel types in the endpoint definitions that were imported to create the segment.\"\n        }\n      ]\n    },\n    \"ExternalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"(Deprecated) Your AWS account ID,\
  \ which you assigned to an external ID key in an IAM trust policy. Amazon Pinpoint previously used this value to assume an IAM role when importing endpoint definitions, but we removed this requirement. We don't recommend use of external IDs for IAM roles that are assumed by Amazon Pinpoint.\"\n        }\n      ]\n    },\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Format\"\n        },\n        {\n          \"description\": \"The format of the files that were imported to create the segment. Valid values are: CSV, for comma-separated values format; and, JSON, for newline-delimited JSON format.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the AWS Identity and Access Management (IAM) role that authorized Amazon Pinpoint to access the Amazon S3 location to import endpoint\
  \ definitions from.\"\n        }\n      ]\n    },\n    \"S3Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The URL of the Amazon Simple Storage Service (Amazon S3) bucket that the endpoint definitions were imported from to create the segment.\"\n        }\n      ]\n    },\n    \"Size\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The number of endpoint definitions that were imported successfully to create the segment.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Format\",\n    \"S3Url\",\n    \"Size\",\n    \"ExternalId\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-segment-import-resource-schema.json
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
title: SegmentImportResource
---
