---
description: <p>The SCTE-35 <code>time_signal</code> message can be sent with one or more <code>segmentation_descriptor</code> messages. A <code>time_signal</code> message can be sent only if a single <code>segmentation_descriptor</code> message is sent.</p> <p>The <code>time_signal</code> message contains only the <code>splice_time</code> field which is constructed using a given presentation timestamp. When sending a <code>time_signal</code> message, the <code>splice_command_type</code> field in the <code>splice_info_section</code> message is set to 6 (0x06).</p> <p>See the <code>time_signal()</code> table of the 2022 SCTE-35 specification for more information.</p>
layout: schema
name: TimeSignalMessage
properties_list:
- description: ''
  name: SegmentationDescriptors
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-time-signal-message-schema.json
slug: mediatailor-api-time-signal-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-time-signal-message-schema.json\",\n  \"title\": \"TimeSignalMessage\",\n  \"description\": \"<p>The SCTE-35 <code>time_signal</code> message can be sent with one or more <code>segmentation_descriptor</code> messages. A <code>time_signal</code> message can be sent only if a single <code>segmentation_descriptor</code> message is sent.</p> <p>The <code>time_signal</code> message contains only the <code>splice_time</code> field which is constructed using a given presentation timestamp. When sending a <code>time_signal</code> message, the <code>splice_command_type</code> field in the <code>splice_info_section</code> message is set to 6 (0x06).</p> <p>See the <code>time_signal()</code> table of the 2022 SCTE-35 specification for more information.</p>\",\n  \"type\": \"object\",\n  \"properties\"\
  : {\n    \"SegmentationDescriptors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SegmentationDescriptorList\"\n        },\n        {\n          \"description\": \"The configurations for the SCTE-35 <code>segmentation_descriptor</code> message(s) sent with the <code>time_signal</code> message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-time-signal-message-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: TimeSignalMessage
---
