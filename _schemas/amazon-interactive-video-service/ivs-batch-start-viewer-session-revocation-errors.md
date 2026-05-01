---
description: BatchStartViewerSessionRevocationErrors schema
layout: schema
name: BatchStartViewerSessionRevocationErrors
properties_list: []
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-start-viewer-session-revocation-errors-schema.json
slug: ivs-batch-start-viewer-session-revocation-errors
source_filename: ivs-batch-start-viewer-session-revocation-errors-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-start-viewer-session-revocation-errors-schema.json\",\n  \"title\": \"BatchStartViewerSessionRevocationErrors\",\n  \"description\": \"BatchStartViewerSessionRevocationErrors schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"channelArn\",\n      \"viewerId\"\n    ],\n    \"properties\": {\n      \"channelArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ChannelArn\"\n          },\n          {\n            \"description\": \"Channel ARN.\"\n          }\n        ]\n      },\n      \"code\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/errorCode\"\n          },\n          {\n            \"description\": \"Error code.\"\n          }\n        ]\n \
  \     },\n      \"message\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/errorMessage\"\n          },\n          {\n            \"description\": \"Error message, determined by the application.\"\n          }\n        ]\n      },\n      \"viewerId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ViewerId\"\n          },\n          {\n            \"description\": \"The ID of the viewer session to revoke.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Error for a request in the batch for BatchStartViewerSessionRevocation. Each error is related to a specific channel-ARN and viewer-ID pair.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-start-viewer-session-revocation-errors-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: BatchStartViewerSessionRevocationErrors
---
