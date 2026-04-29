---
description: Description of the source and destination queues between which the job has moved, along with the timestamp of the move
layout: schema
name: QueueTransition
properties_list:
- description: ''
  name: DestinationQueue
  type: object
- description: ''
  name: SourceQueue
  type: object
- description: ''
  name: Timestamp
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-queue-transition-schema.json
slug: mediaconvert-api-queue-transition
source_filename: mediaconvert-api-queue-transition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-queue-transition-schema.json\",\n  \"title\": \"QueueTransition\",\n  \"description\": \"Description of the source and destination queues between which the job has moved, along with the timestamp of the move\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationQueue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationQueue\"\n          },\n          \"description\": \"The queue that the job was on after the transition.\"\n        }\n      ]\n    },\n    \"SourceQueue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceQueue\"\n         \
  \ },\n          \"description\": \"The queue that the job was on before the transition.\"\n        }\n      ]\n    },\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampUnix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timestamp\"\n          },\n          \"description\": \"The time, in Unix epoch format, that the job moved from the source queue to the destination queue.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-queue-transition-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: QueueTransition
---
