---
description: Caption Destination Settings
layout: schema
name: CaptionDestinationSettings
properties_list:
- description: ''
  name: AribDestinationSettings
  type: object
- description: ''
  name: BurnInDestinationSettings
  type: object
- description: ''
  name: DvbSubDestinationSettings
  type: object
- description: ''
  name: EbuTtDDestinationSettings
  type: object
- description: ''
  name: EmbeddedDestinationSettings
  type: object
- description: ''
  name: EmbeddedPlusScte20DestinationSettings
  type: object
- description: ''
  name: RtmpCaptionInfoDestinationSettings
  type: object
- description: ''
  name: Scte20PlusEmbeddedDestinationSettings
  type: object
- description: ''
  name: Scte27DestinationSettings
  type: object
- description: ''
  name: SmpteTtDestinationSettings
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
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-caption-destination-settings-schema.json
slug: medialive-api-caption-destination-settings
source_filename: medialive-api-caption-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-destination-settings-schema.json\",\n  \"title\": \"CaptionDestinationSettings\",\n  \"description\": \"Caption Destination Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AribDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AribDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"aribDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"BurnInDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurnInDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"burnInDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"DvbSubDestinationSettings\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSubDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"EbuTtDDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbuTtDDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebuTtDDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"EmbeddedDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmbeddedDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"embeddedDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"EmbeddedPlusScte20DestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmbeddedPlusScte20DestinationSettings\"\n        },\n        {\n          \"xml\":\
  \ {\n            \"name\": \"embeddedPlusScte20DestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"RtmpCaptionInfoDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RtmpCaptionInfoDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rtmpCaptionInfoDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"Scte20PlusEmbeddedDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte20PlusEmbeddedDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte20PlusEmbeddedDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"Scte27DestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte27DestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte27DestinationSettings\"\n          }\n        }\n  \
  \    ]\n    },\n    \"SmpteTtDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmpteTtDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"smpteTtDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"TeletextDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TeletextDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"teletextDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"TtmlDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TtmlDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ttmlDestinationSettings\"\n          }\n        }\n      ]\n    },\n    \"WebvttDestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebvttDestinationSettings\"\n\
  \        },\n        {\n          \"xml\": {\n            \"name\": \"webvttDestinationSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CaptionDestinationSettings
---
