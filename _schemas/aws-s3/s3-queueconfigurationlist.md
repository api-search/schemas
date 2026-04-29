---
description: ''
layout: schema
name: QueueConfigurationList
properties_list: []
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-queueconfigurationlist-schema.json
slug: s3-queueconfigurationlist
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueueConfigurationList\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Id\": {\n        \"type\": \"string\",\n        \"description\": \"An optional unique identifier for configurations in a notification configuration. If you don't provide one, Amazon S3 will assign an ID.\"\n      },\n      \"QueueArn\": {},\n      \"Events\": {},\n      \"Filter\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Key\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/S3KeyFilter\"\n              },\n              {\n                \"xml\": {\n                  \"name\": \"S3Key\"\n                }\n              }\n            ]\n          }\n        },\n        \"description\": \"Specifies object key name filtering rules. For information about key name filtering, see <a href=\\\"\
  https://docs.aws.amazon.com/AmazonS3/latest/dev/NotificationHowTo.html\\\">Configuring Event Notifications</a> in the <i>Amazon S3 User Guide</i>.\"\n      }\n    },\n    \"required\": [\n      \"QueueArn\",\n      \"Events\"\n    ],\n    \"description\": \"Specifies the configuration for publishing messages to an Amazon Simple Queue Service (Amazon SQS) queue when Amazon S3 detects specified events.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-queueconfigurationlist-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: QueueConfigurationList
---
