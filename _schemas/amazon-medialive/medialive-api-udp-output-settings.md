---
description: Udp Output Settings
layout: schema
name: UdpOutputSettings
properties_list:
- description: ''
  name: BufferMsec
  type: object
- description: ''
  name: ContainerSettings
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: FecOutputSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-udp-output-settings-schema.json
slug: medialive-api-udp-output-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-udp-output-settings-schema.json\",\n  \"title\": \"UdpOutputSettings\",\n  \"description\": \"Udp Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BufferMsec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max10000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bufferMsec\"\n          },\n          \"description\": \"UDP output buffering in milliseconds. Larger values increase latency through the transcoder but simultaneously assist the transcoder in maintaining a constant, low-jitter UDP/RTP output while accommodating clock recovery, input switching, input disruptions, picture reordering, etc.\"\n        }\n      ]\n    },\n    \"ContainerSettings\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/UdpContainerSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"containerSettings\"\n          }\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputLocationRef\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"Destination address and port number for RTP or UDP packets. Can be unicast or multicast RTP or UDP (eg. rtp://239.10.10.10:5001 or udp://10.100.100.100:5002).\"\n        }\n      ]\n    },\n    \"FecOutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FecOutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fecOutputSettings\"\n          },\n          \"description\": \"Settings for enabling and adjusting Forward Error Correction on UDP outputs.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"Destination\",\n    \"ContainerSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-udp-output-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UdpOutputSettings
---
