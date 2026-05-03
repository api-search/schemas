---
description: Schema representing a live stream on a Red5 Pro server, including publishing configuration, subscriber tracking, and media codec details.
layout: schema
name: Red5 Pro Stream
properties_list:
- description: Unique stream name identifier within the application scope
  name: name
  type: string
- description: Red5 Pro application scope that contains this stream
  name: appName
  type: string
- description: Identifier of the publishing client connection
  name: clientId
  type: string
- description: Current operational status of the stream
  name: status
  type: string
- description: Streaming protocol used by the publisher
  name: protocol
  type: string
- description: Stream duration in milliseconds since publishing began
  name: duration
  type: integer
- description: Number of currently active subscribers to this stream
  name: subscriberCount
  type: integer
- description: Total bytes received from the publisher
  name: bytesIn
  type: integer
- description: Total bytes sent to all subscribers
  name: bytesOut
  type: integer
- description: ''
  name: video
  type: object
- description: ''
  name: audio
  type: object
- description: ''
  name: recording
  type: object
provider_name: Red5
provider_slug: red5
schema_file: json-schema/red5-stream-schema.json
slug: red5-stream
source_filename: red5-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.red5.net/schemas/stream.json\",\n  \"title\": \"Red5 Pro Stream\",\n  \"description\": \"Schema representing a live stream on a Red5 Pro server, including publishing configuration, subscriber tracking, and media codec details.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique stream name identifier within the application scope\",\n      \"maxLength\": 255\n    },\n    \"appName\": {\n      \"type\": \"string\",\n      \"description\": \"Red5 Pro application scope that contains this stream\",\n      \"default\": \"live\"\n    },\n    \"clientId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the publishing client connection\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of the stream\",\n\
  \      \"enum\": [\"publishing\", \"idle\", \"error\"]\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Streaming protocol used by the publisher\",\n      \"enum\": [\"rtmp\", \"webrtc\", \"rtsp\", \"srt\"]\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Stream duration in milliseconds since publishing began\",\n      \"minimum\": 0\n    },\n    \"subscriberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of currently active subscribers to this stream\",\n      \"minimum\": 0\n    },\n    \"bytesIn\": {\n      \"type\": \"integer\",\n      \"description\": \"Total bytes received from the publisher\",\n      \"minimum\": 0\n    },\n    \"bytesOut\": {\n      \"type\": \"integer\",\n      \"description\": \"Total bytes sent to all subscribers\",\n      \"minimum\": 0\n    },\n    \"video\": {\n      \"$ref\": \"#/$defs/VideoTrack\"\n    },\n    \"audio\": {\n      \"$ref\": \"#/$defs/AudioTrack\"\
  \n    },\n    \"recording\": {\n      \"$ref\": \"#/$defs/RecordingConfig\"\n    }\n  },\n  \"$defs\": {\n    \"VideoTrack\": {\n      \"type\": \"object\",\n      \"description\": \"Video track properties for a live stream\",\n      \"properties\": {\n        \"codec\": {\n          \"type\": \"string\",\n          \"description\": \"Video codec identifier (e.g., H264, H265, VP8)\",\n          \"examples\": [\"H264\", \"H265\", \"VP8\", \"VP9\"]\n        },\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"Video frame width in pixels\",\n          \"minimum\": 1,\n          \"maximum\": 7680\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"Video frame height in pixels\",\n          \"minimum\": 1,\n          \"maximum\": 4320\n        },\n        \"frameRate\": {\n          \"type\": \"number\",\n          \"description\": \"Video frame rate in frames per second\",\n          \"minimum\": 1,\n      \
  \    \"maximum\": 120\n        },\n        \"bitrate\": {\n          \"type\": \"integer\",\n          \"description\": \"Video bitrate in bits per second\",\n          \"minimum\": 0\n        },\n        \"keyFrameInterval\": {\n          \"type\": \"number\",\n          \"description\": \"Interval between keyframes in seconds\"\n        }\n      }\n    },\n    \"AudioTrack\": {\n      \"type\": \"object\",\n      \"description\": \"Audio track properties for a live stream\",\n      \"properties\": {\n        \"codec\": {\n          \"type\": \"string\",\n          \"description\": \"Audio codec identifier (e.g., AAC, MP3, Opus)\",\n          \"examples\": [\"AAC\", \"MP3\", \"Opus\", \"Speex\"]\n        },\n        \"sampleRate\": {\n          \"type\": \"integer\",\n          \"description\": \"Audio sample rate in Hz\",\n          \"enum\": [8000, 11025, 16000, 22050, 32000, 44100, 48000]\n        },\n        \"channels\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Number of audio channels (1 for mono, 2 for stereo)\",\n          \"minimum\": 1,\n          \"maximum\": 8\n        },\n        \"bitrate\": {\n          \"type\": \"integer\",\n          \"description\": \"Audio bitrate in bits per second\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"RecordingConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for stream recording\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether recording is currently active for this stream\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\": \"Recording file format\",\n          \"enum\": [\"mp4\", \"flv\"]\n        },\n        \"filePath\": {\n          \"type\": \"string\",\n          \"description\": \"Server filesystem path where the recording is saved\"\n        },\n        \"startTime\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\",\n          \"description\": \"Timestamp when recording started\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red5/refs/heads/main/json-schema/red5-stream-schema.json
tags:
- Live Streaming
- Media
- Real-Time
- RTMP
- Streaming
- Video
- WebRTC
title: Red5 Pro Stream
---
