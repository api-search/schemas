---
description: A key pair used to sign and validate a playback authorization token.
layout: schema
name: PlaybackKeyPair
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: fingerprint
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-playback-key-pair-schema.json
slug: ivs-playback-key-pair
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-playback-key-pair-schema.json\",\n  \"title\": \"PlaybackKeyPair\",\n  \"description\": \"A key pair used to sign and validate a playback authorization token.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackKeyPairArn\"\n        },\n        {\n          \"description\": \"Key-pair ARN.\"\n        }\n      ]\n    },\n    \"fingerprint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackKeyPairFingerprint\"\n        },\n        {\n          \"description\": \"Key-pair identifier.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackKeyPairName\"\n        },\n        {\n    \
  \      \"description\": \"Playback-key-pair name. The value does not need to be unique.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"Tags attached to the resource. Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \\\"Tag naming limits and requirements\\\"; Amazon IVS has no service-specific constraints beyond what is documented there.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-playback-key-pair-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: PlaybackKeyPair
---
