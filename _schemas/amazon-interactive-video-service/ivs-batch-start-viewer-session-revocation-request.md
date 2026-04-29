---
description: BatchStartViewerSessionRevocationRequest schema
layout: schema
name: BatchStartViewerSessionRevocationRequest
properties_list:
- description: ''
  name: viewerSessions
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-batch-start-viewer-session-revocation-request-schema.json
slug: ivs-batch-start-viewer-session-revocation-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-start-viewer-session-revocation-request-schema.json\",\n  \"title\": \"BatchStartViewerSessionRevocationRequest\",\n  \"description\": \"BatchStartViewerSessionRevocationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"viewerSessions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchStartViewerSessionRevocationViewerSessionList\"\n        },\n        {\n          \"description\": \"Array of viewer sessions, one per channel-ARN and viewer-ID pair.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"viewerSessions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-batch-start-viewer-session-revocation-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: BatchStartViewerSessionRevocationRequest
---
