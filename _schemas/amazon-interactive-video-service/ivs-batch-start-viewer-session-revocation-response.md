---
description: BatchStartViewerSessionRevocationResponse schema
layout: schema
name: BatchStartViewerSessionRevocationResponse
properties_list:
- description: ''
  name: errors
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-start-viewer-session-revocation-response-schema.json
slug: ivs-batch-start-viewer-session-revocation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-start-viewer-session-revocation-response-schema.json\",\n  \"title\": \"BatchStartViewerSessionRevocationResponse\",\n  \"description\": \"BatchStartViewerSessionRevocationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchStartViewerSessionRevocationErrors\"\n        },\n        {\n          \"description\": \"Each error object is related to a specific <code>channelArn</code> and <code>viewerId</code> pair in the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-start-viewer-session-revocation-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: BatchStartViewerSessionRevocationResponse
---
