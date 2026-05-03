---
description: Represents an RTSP streaming session as defined by RFC 7826
layout: schema
name: RTSP Session
properties_list:
- description: Unique session identifier assigned by the server (Session header value)
  name: sessionId
  type: string
- description: RTSP URL for the stream (rtsp://host:port/path)
  name: url
  type: string
- description: Current session state
  name: state
  type: string
- description: Transport specification (e.g., RTP/AVP;unicast;client_port=4588-4589)
  name: transport
  type: string
- description: Server RTP/RTCP port pair (e.g., 6256-6257)
  name: serverPort
  type: string
- description: Client RTP/RTCP port pair (e.g., 4588-4589)
  name: clientPort
  type: string
- description: Session timeout in seconds
  name: timeout
  type: integer
- description: Session Description Protocol (SDP) content describing the media
  name: sdp
  type: string
provider_name: RTSP
provider_slug: rtsp
schema_file: json-schema/rtsp-session-schema.json
slug: rtsp-session
source_filename: rtsp-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://datatracker.ietf.org/schemas/rtsp/session\",\n  \"title\": \"RTSP Session\",\n  \"description\": \"Represents an RTSP streaming session as defined by RFC 7826\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique session identifier assigned by the server (Session header value)\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"pattern\": \"^rtsp://\",\n      \"description\": \"RTSP URL for the stream (rtsp://host:port/path)\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current session state\",\n      \"enum\": [\"Init\", \"Ready\", \"Playing\", \"Recording\"]\n    },\n    \"transport\": {\n      \"type\": \"string\",\n      \"description\": \"Transport specification (e.g., RTP/AVP;unicast;client_port=4588-4589)\"\n    },\n    \"serverPort\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Server RTP/RTCP port pair (e.g., 6256-6257)\"\n    },\n    \"clientPort\": {\n      \"type\": \"string\",\n      \"description\": \"Client RTP/RTCP port pair (e.g., 4588-4589)\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Session timeout in seconds\",\n      \"minimum\": 0\n    },\n    \"sdp\": {\n      \"type\": \"string\",\n      \"description\": \"Session Description Protocol (SDP) content describing the media\"\n    }\n  },\n  \"required\": [\"sessionId\", \"url\", \"state\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rtsp/refs/heads/main/json-schema/rtsp-session-schema.json
tags:
- Streaming
- Video
- Media
- Protocol
- Real-Time
title: RTSP Session
---
