---
description: UpdateQueueResponse schema from Amazon MediaConvert API
layout: schema
name: UpdateQueueResponse
properties_list:
- description: ''
  name: Queue
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-update-queue-response-schema.json
slug: mediaconvert-api-update-queue-response
source_filename: mediaconvert-api-update-queue-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-queue-response-schema.json\",\n  \"title\": \"UpdateQueueResponse\",\n  \"description\": \"UpdateQueueResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Queue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Queue\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"queue\"\n          },\n          \"description\": \"You can use queues to manage the resources that are available to your AWS account for running multiple transcoding jobs at the same time. If you don't specify a queue, the service sends all jobs through the default queue. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/working-with-queues.html.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-update-queue-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateQueueResponse
---
