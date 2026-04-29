---
description: BatchStartViewerSessionRevocationViewerSessionList schema
layout: schema
name: BatchStartViewerSessionRevocationViewerSessionList
properties_list: []
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-start-viewer-session-revocation-viewer-session-list-schema.json
slug: ivs-batch-start-viewer-session-revocation-viewer-session-list
source_filename: ivs-batch-start-viewer-session-revocation-viewer-session-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-start-viewer-session-revocation-viewer-session-list-schema.json\",\n  \"title\": \"BatchStartViewerSessionRevocationViewerSessionList\",\n  \"description\": \"BatchStartViewerSessionRevocationViewerSessionList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"channelArn\",\n      \"viewerId\"\n    ],\n    \"properties\": {\n      \"channelArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ChannelArn\"\n          },\n          {\n            \"description\": \"The ARN of the channel associated with the viewer session to revoke.\"\n          }\n        ]\n      },\n      \"viewerId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ViewerId\"\n    \
  \      },\n          {\n            \"description\": \"The ID of the viewer associated with the viewer session to revoke. Do not use this field for personally identifying, confidential, or sensitive information.\"\n          }\n        ]\n      },\n      \"viewerSessionVersionsLessThanOrEqualTo\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ViewerSessionVersion\"\n          },\n          {\n            \"description\": \"An optional filter on which versions of the viewer session to revoke. All versions less than or equal to the specified version will be revoked. Default: 0.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A viewer session to revoke in the call to <a>BatchStartViewerSessionRevocation</a>.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-start-viewer-session-revocation-viewer-session-list-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: BatchStartViewerSessionRevocationViewerSessionList
---
