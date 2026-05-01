---
description: ImportPlaybackKeyPairRequest schema
layout: schema
name: ImportPlaybackKeyPairRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: publicKeyMaterial
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-import-playback-key-pair-request-schema.json
slug: ivs-import-playback-key-pair-request
source_filename: ivs-import-playback-key-pair-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-import-playback-key-pair-request-schema.json\",\n  \"title\": \"ImportPlaybackKeyPairRequest\",\n  \"description\": \"ImportPlaybackKeyPairRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackKeyPairName\"\n        },\n        {\n          \"description\": \"Playback-key-pair name. The value does not need to be unique.\"\n        }\n      ]\n    },\n    \"publicKeyMaterial\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackPublicKeyMaterial\"\n        },\n        {\n          \"description\": \"The public portion of a customer-generated key pair.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"Any tags provided with the request are added to the playback key pair tags. See <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \\\"Tag naming limits and requirements\\\"; Amazon IVS has no service-specific constraints beyond what is documented there.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"publicKeyMaterial\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-import-playback-key-pair-request-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: ImportPlaybackKeyPairRequest
---
