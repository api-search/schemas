---
description: Udp Group Settings
layout: schema
name: UdpGroupSettings
properties_list:
- description: ''
  name: InputLossAction
  type: object
- description: ''
  name: TimedMetadataId3Frame
  type: object
- description: ''
  name: TimedMetadataId3Period
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-udp-group-settings-schema.json
slug: medialive-api-udp-group-settings
source_filename: medialive-api-udp-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-udp-group-settings-schema.json\",\n  \"title\": \"UdpGroupSettings\",\n  \"description\": \"Udp Group Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputLossAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLossActionForUdpOut\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputLossAction\"\n          },\n          \"description\": \"Specifies behavior of last resort when input video is lost, and no more backup inputs are available. When dropTs is selected the entire transport stream will stop being emitted.  When dropProgram is selected the program can be dropped from the transport stream (and replaced with null packets to meet the TS bitrate requirement).  Or, when emitProgram is chosen the transport\
  \ stream will continue to be produced normally with repeat frames, black frames, or slate frames substituted for the absent input video.\"\n        }\n      ]\n    },\n    \"TimedMetadataId3Frame\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UdpTimedMetadataId3Frame\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataId3Frame\"\n          },\n          \"description\": \"Indicates ID3 frame that has the timecode.\"\n        }\n      ]\n    },\n    \"TimedMetadataId3Period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataId3Period\"\n          },\n          \"description\": \"Timed Metadata interval in seconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-udp-group-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UdpGroupSettings
---
