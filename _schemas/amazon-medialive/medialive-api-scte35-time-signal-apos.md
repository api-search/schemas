---
description: Atypical configuration that applies segment breaks only on SCTE-35 time signal placement opportunities and breaks.
layout: schema
name: Scte35TimeSignalApos
properties_list:
- description: ''
  name: AdAvailOffset
  type: object
- description: ''
  name: NoRegionalBlackoutFlag
  type: object
- description: ''
  name: WebDeliveryAllowedFlag
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-time-signal-apos-schema.json
slug: medialive-api-scte35-time-signal-apos
source_filename: medialive-api-scte35-time-signal-apos-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-time-signal-apos-schema.json\",\n  \"title\": \"Scte35TimeSignalApos\",\n  \"description\": \"Atypical configuration that applies segment breaks only on SCTE-35 time signal placement opportunities and breaks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdAvailOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative1000Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adAvailOffset\"\n          },\n          \"description\": \"When specified, this offset (in milliseconds) is added to the input Ad Avail PTS time. This only applies to embedded SCTE 104/35 messages and does not apply to OOB messages.\"\n        }\n      ]\n    },\n    \"NoRegionalBlackoutFlag\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/Scte35AposNoRegionalBlackoutBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"noRegionalBlackoutFlag\"\n          },\n          \"description\": \"When set to ignore, Segment Descriptors with noRegionalBlackoutFlag set to 0 will no longer trigger blackouts or Ad Avail slates\"\n        }\n      ]\n    },\n    \"WebDeliveryAllowedFlag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35AposWebDeliveryAllowedBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"webDeliveryAllowedFlag\"\n          },\n          \"description\": \"When set to ignore, Segment Descriptors with webDeliveryAllowedFlag set to 0 will no longer trigger blackouts or Ad Avail slates\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-time-signal-apos-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Scte35TimeSignalApos
---
