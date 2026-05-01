---
description: Specifies settings for publishing event data to an Amazon Kinesis data stream or an Amazon Kinesis Data Firehose delivery stream.
layout: schema
name: EventStream
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: DestinationStreamArn
  type: object
- description: ''
  name: ExternalId
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: LastUpdatedBy
  type: object
- description: ''
  name: RoleArn
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-event-stream-schema.json
slug: amazon-pinpoint-event-stream
source_filename: amazon-pinpoint-event-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-stream-schema.json\",\n  \"title\": \"EventStream\",\n  \"description\": \"Specifies settings for publishing event data to an Amazon Kinesis data stream or an Amazon Kinesis Data Firehose delivery stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application to publish event data for.\"\n        }\n      ]\n    },\n    \"DestinationStreamArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the Amazon Kinesis data stream or Amazon Kinesis Data Firehose delivery\
  \ stream to publish event data to.</p> <p>For a Kinesis data stream, the ARN format is: arn:aws:kinesis:<replaceable>region</replaceable>:<replaceable>account-id</replaceable>:stream/<replaceable>stream_name</replaceable>\\n               </p> <p>For a Kinesis Data Firehose delivery stream, the ARN format is: arn:aws:firehose:<replaceable>region</replaceable>:<replaceable>account-id</replaceable>:deliverystream/<replaceable>stream_name</replaceable>\\n               </p>\"\n        }\n      ]\n    },\n    \"ExternalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"(Deprecated) Your AWS account ID, which you assigned to an external ID key in an IAM trust policy. Amazon Pinpoint previously used this value to assume an IAM role when publishing event data, but we removed this requirement. We don't recommend use of external IDs for IAM roles that are assumed by Amazon Pinpoint.\"\n        }\n  \
  \    ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the event stream was last modified.\"\n        }\n      ]\n    },\n    \"LastUpdatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The IAM user who last modified the event stream.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The AWS Identity and Access Management (IAM) role that authorizes Amazon Pinpoint to publish event data to the stream in your AWS account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationId\",\n    \"RoleArn\",\n    \"DestinationStreamArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-stream-schema.json
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
title: EventStream
---
