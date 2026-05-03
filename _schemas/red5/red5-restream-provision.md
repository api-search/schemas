---
description: Schema representing a restreaming provision that configures the Red5 Pro server to forward a live stream to one or more external RTMP, RTMPS, SRT, or Zixi destinations.
layout: schema
name: Red5 Pro Restream Provision
properties_list:
- description: Name of the source live stream to retransmit
  name: streamName
  type: string
- description: Red5 Pro application scope containing the source stream
  name: appName
  type: string
- description: 'Restreaming mode: push sends to external destinations, pull ingests from external sources'
  name: type
  type: string
- description: Current operational status of this restream provision
  name: status
  type: string
- description: External RTMP/RTMPS destinations to push the stream to (used for push type)
  name: destinations
  type: array
- description: ''
  name: source
  type: object
- description: ''
  name: fileConfig
  type: object
- description: ''
  name: reconnect
  type: object
provider_name: Red5
provider_slug: red5
schema_file: json-schema/red5-restream-provision-schema.json
slug: red5-restream-provision
source_filename: red5-restream-provision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.red5.net/schemas/restream-provision.json\",\n  \"title\": \"Red5 Pro Restream Provision\",\n  \"description\": \"Schema representing a restreaming provision that configures the Red5 Pro server to forward a live stream to one or more external RTMP, RTMPS, SRT, or Zixi destinations.\",\n  \"type\": \"object\",\n  \"required\": [\"streamName\", \"type\"],\n  \"properties\": {\n    \"streamName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the source live stream to retransmit\",\n      \"maxLength\": 255\n    },\n    \"appName\": {\n      \"type\": \"string\",\n      \"description\": \"Red5 Pro application scope containing the source stream\",\n      \"default\": \"live\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Restreaming mode: push sends to external destinations, pull ingests from external sources\",\n      \"enum\": [\"push\"\
  , \"pull\", \"file\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of this restream provision\",\n      \"enum\": [\"active\", \"stopped\", \"error\", \"connecting\"]\n    },\n    \"destinations\": {\n      \"type\": \"array\",\n      \"description\": \"External RTMP/RTMPS destinations to push the stream to (used for push type)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Destination\"\n      }\n    },\n    \"source\": {\n      \"$ref\": \"#/$defs/Source\"\n    },\n    \"fileConfig\": {\n      \"$ref\": \"#/$defs/FileConfig\"\n    },\n    \"reconnect\": {\n      \"$ref\": \"#/$defs/ReconnectConfig\"\n    }\n  },\n  \"$defs\": {\n    \"Destination\": {\n      \"type\": \"object\",\n      \"description\": \"An external destination endpoint for RTMP push restreaming\",\n      \"required\": [\"url\", \"streamKey\"],\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"RTMP or RTMPS ingest URL of the destination platform\",\n          \"pattern\": \"^rtmps?://\",\n          \"examples\": [\n            \"rtmp://a.rtmp.youtube.com/live2\",\n            \"rtmps://live-api-s.facebook.com:443/rtmp/\"\n          ]\n        },\n        \"streamKey\": {\n          \"type\": \"string\",\n          \"description\": \"Stream key provided by the destination platform\",\n          \"minLength\": 1\n        },\n        \"protocol\": {\n          \"type\": \"string\",\n          \"description\": \"Transport protocol for this destination\",\n          \"enum\": [\"rtmp\", \"rtmps\"],\n          \"default\": \"rtmp\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable label for this destination (e.g., YouTube, Facebook)\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this destination is currently active\",\n          \"default\": true\n     \
  \   }\n      }\n    },\n    \"Source\": {\n      \"type\": \"object\",\n      \"description\": \"External RTMP source configuration for pull restreaming\",\n      \"required\": [\"url\"],\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"RTMP URL of the external source to pull from\",\n          \"pattern\": \"^rtmps?://\"\n        },\n        \"streamKey\": {\n          \"type\": \"string\",\n          \"description\": \"Stream key at the source if required for authentication\"\n        }\n      }\n    },\n    \"FileConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for file-based pseudo-live restreaming\",\n      \"required\": [\"filePath\"],\n      \"properties\": {\n        \"filePath\": {\n          \"type\": \"string\",\n          \"description\": \"Server filesystem path to the FLV or MP4 file to restream\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"File format of the source file\",\n          \"enum\": [\"flv\", \"mp4\"]\n        },\n        \"loop\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to loop the file when playback reaches the end\",\n          \"default\": false\n        }\n      }\n    },\n    \"ReconnectConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Automatic reconnection settings for a restream provision\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to automatically reconnect if the connection is lost\",\n          \"default\": true\n        },\n        \"maxAttempts\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of reconnection attempts before giving up\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"default\": 5\n        },\n        \"delayMs\": {\n          \"type\": \"integer\",\n          \"description\": \"Delay in milliseconds\
  \ between reconnection attempts\",\n          \"minimum\": 100,\n          \"default\": 5000\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/json-schema/red5-restream-provision-schema.json
tags:
- Live Streaming
- Media
- Real-Time
- RTMP
- Streaming
- Video
- WebRTC
title: Red5 Pro Restream Provision
---
