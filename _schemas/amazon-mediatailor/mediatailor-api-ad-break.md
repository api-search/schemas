---
description: Ad break configuration parameters.
layout: schema
name: AdBreak
properties_list:
- description: ''
  name: MessageType
  type: object
- description: ''
  name: OffsetMillis
  type: object
- description: ''
  name: Slate
  type: object
- description: ''
  name: SpliceInsertMessage
  type: object
- description: ''
  name: TimeSignalMessage
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-ad-break-schema.json
slug: mediatailor-api-ad-break
source_filename: mediatailor-api-ad-break-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-ad-break-schema.json\",\n  \"title\": \"AdBreak\",\n  \"description\": \"Ad break configuration parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MessageType\"\n        },\n        {\n          \"description\": \"The SCTE-35 ad insertion type. Accepted value: <code>SPLICE_INSERT</code>, <code>TIME_SIGNAL</code>.\"\n        }\n      ]\n    },\n    \"OffsetMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"How long (in milliseconds) after the beginning of the program that an ad starts. This value must fall within 100ms of a segment boundary, otherwise the ad break will be skipped.\"\
  \n        }\n      ]\n    },\n    \"Slate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SlateSource\"\n        },\n        {\n          \"description\": \"Ad break slate configuration.\"\n        }\n      ]\n    },\n    \"SpliceInsertMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpliceInsertMessage\"\n        },\n        {\n          \"description\": \"This defines the SCTE-35 <code>splice_insert()</code> message inserted around the ad. For information about using <code>splice_insert()</code>, see the SCTE-35 specficiaiton, section 9.7.3.1.\"\n        }\n      ]\n    },\n    \"TimeSignalMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSignalMessage\"\n        },\n        {\n          \"description\": \"<p>Defines the SCTE-35 <code>time_signal</code> message inserted around the ad.</p> <p>Programs on a channel's schedule can be configured with one or more ad breaks. You\
  \ can attach a <code>splice_insert</code> SCTE-35 message to the ad break. This message provides basic metadata about the ad break.</p> <p>See section 9.7.4 of the 2022 SCTE-35 specification for more information.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-ad-break-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AdBreak
---
