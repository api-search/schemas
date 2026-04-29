---
description: A container for specifying the configuration for publication of messages to an Amazon Simple Notification Service (Amazon SNS) topic when Amazon S3 detects specified events. This data type is deprecated. Use <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_TopicConfiguration.html">TopicConfiguration</a> instead.
layout: schema
name: TopicConfigurationDeprecated
properties_list:
- description: An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.
  name: Id
  type: string
- description: ''
  name: Events
  type: object
- description: ''
  name: Event
  type: object
- description: ''
  name: Topic
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-topicconfigurationdeprecated-schema.json
slug: s3-topicconfigurationdeprecated
source_filename: s3-topicconfigurationdeprecated-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TopicConfigurationDeprecated\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.\"\n    },\n    \"Events\": {},\n    \"Event\": {},\n    \"Topic\": {}\n  },\n  \"description\": \"A container for specifying the configuration for publication of messages to an Amazon Simple Notification Service (Amazon SNS) topic when Amazon S3 detects specified events. This data type is deprecated. Use <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_TopicConfiguration.html\\\">TopicConfiguration</a> instead.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-topicconfigurationdeprecated-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: TopicConfigurationDeprecated
---
