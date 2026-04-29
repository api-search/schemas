---
description: Settings related to one captions tab on the MediaConvert console. In your job JSON, an instance of captions DestinationSettings is equivalent to one captions tab in the console. Usually, one captions tab corresponds to one output captions track. Depending on your output captions format, one tab might correspond to a set of output captions tracks. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/including-captions.html.
layout: schema
name: CaptionDestinationSettings
properties_list:
- description: ''
  name: BurninDestinationSettings
  type: object
- description: ''
  name: DestinationType
  type: object
- description: ''
  name: DvbSubDestinationSettings
  type: object
- description: ''
  name: EmbeddedDestinationSettings
  type: object
- description: ''
  name: ImscDestinationSettings
  type: object
- description: ''
  name: SccDestinationSettings
  type: object
- description: ''
  name: SrtDestinationSettings
  type: object
- description: ''
  name: TeletextDestinationSettings
  type: object
- description: ''
  name: TtmlDestinationSettings
  type: object
- description: ''
  name: WebvttDestinationSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-caption-destination-settings-schema.json
slug: mediaconvert-api-caption-destination-settings
source_filename: mediaconvert-api-caption-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-destination-settings-schema.json\",\n  \"title\": \"CaptionDestinationSettings\",\n  \"description\": \"Settings related to one captions tab on the MediaConvert console. In your job JSON, an instance of captions DestinationSettings is equivalent to one captions tab in the console. Usually, one captions tab corresponds to one output captions track. Depending on your output captions format, one tab might correspond to a set of output captions tracks. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/including-captions.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BurninDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninDestinationSettings\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"burninDestinationSettings\"\n          },\n          \"description\": \"Burn-in is a captions delivery method, rather than a captions format. Burn-in writes the captions directly on your video frames, replacing pixels of video content with the captions. Set up burn-in captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/burn-in-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to BURN_IN.\"\n        }\n      ]\n    },\n    \"DestinationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionDestinationType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationType\"\n          },\n          \"description\": \"Specify the format for this set of captions on this output. The default format is embedded without SCTE-20. Note that your\
  \ choice of video output container constrains your choice of output captions format. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/captions-support-tables.html. If you are using SCTE-20 and you want to create an output that complies with the SCTE-43 spec, choose SCTE-20 plus embedded (SCTE20_PLUS_EMBEDDED). To create a non-compliant output where the embedded captions come first, choose Embedded plus SCTE-20 (EMBEDDED_PLUS_SCTE20).\"\n        }\n      ]\n    },\n    \"DvbSubDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSubDestinationSettings\"\n          },\n          \"description\": \"Settings related to DVB-Sub captions. Set up DVB-Sub captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/dvb-sub-output-captions.html. When you work directly\
  \ in your JSON job specification, include this object and any required children when you set destinationType to DVB_SUB.\"\n        }\n      ]\n    },\n    \"EmbeddedDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmbeddedDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"embeddedDestinationSettings\"\n          },\n          \"description\": \"Settings related to CEA/EIA-608 and CEA/EIA-708 (also called embedded or ancillary) captions. Set up embedded captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/embedded-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to EMBEDDED, EMBEDDED_PLUS_SCTE20, or SCTE20_PLUS_EMBEDDED.\"\n        }\n      ]\n    },\n    \"ImscDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/ImscDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imscDestinationSettings\"\n          },\n          \"description\": \"Settings related to IMSC captions. IMSC is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to IMSC.\"\n        }\n      ]\n    },\n    \"SccDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SccDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sccDestinationSettings\"\n          },\n          \"description\": \"Settings related to SCC\
  \ captions. SCC is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/scc-srt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to SCC.\"\n        }\n      ]\n    },\n    \"SrtDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SrtDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"srtDestinationSettings\"\n          },\n          \"description\": \"Settings related to SRT captions. SRT is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. When you work directly in your JSON\
  \ job specification, include this object and any required children when you set destinationType to SRT.\"\n        }\n      ]\n    },\n    \"TeletextDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TeletextDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"teletextDestinationSettings\"\n          },\n          \"description\": \"Settings related to teletext captions. Set up teletext captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/teletext-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to TELETEXT.\"\n        }\n      ]\n    },\n    \"TtmlDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TtmlDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"ttmlDestinationSettings\"\n          },\n          \"description\": \"Settings related to TTML captions. TTML is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to TTML.\"\n        }\n      ]\n    },\n    \"WebvttDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebvttDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"webvttDestinationSettings\"\n          },\n          \"description\": \"Settings related to WebVTT captions. WebVTT is a sidecar format that holds captions in a file that is separate from the video container.\
  \ Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to WebVTT.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CaptionDestinationSettings
---
