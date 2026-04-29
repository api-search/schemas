---
description: Caption Selector Settings
layout: schema
name: CaptionSelectorSettings
properties_list:
- description: ''
  name: AncillarySourceSettings
  type: object
- description: ''
  name: AribSourceSettings
  type: object
- description: ''
  name: DvbSubSourceSettings
  type: object
- description: ''
  name: EmbeddedSourceSettings
  type: object
- description: ''
  name: Scte20SourceSettings
  type: object
- description: ''
  name: Scte27SourceSettings
  type: object
- description: ''
  name: TeletextSourceSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-caption-selector-settings-schema.json
slug: medialive-api-caption-selector-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-selector-settings-schema.json\",\n  \"title\": \"CaptionSelectorSettings\",\n  \"description\": \"Caption Selector Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AncillarySourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AncillarySourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ancillarySourceSettings\"\n          }\n        }\n      ]\n    },\n    \"AribSourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AribSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"aribSourceSettings\"\n          }\n        }\n      ]\n    },\n    \"DvbSubSourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/DvbSubSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSubSourceSettings\"\n          }\n        }\n      ]\n    },\n    \"EmbeddedSourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmbeddedSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"embeddedSourceSettings\"\n          }\n        }\n      ]\n    },\n    \"Scte20SourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte20SourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte20SourceSettings\"\n          }\n        }\n      ]\n    },\n    \"Scte27SourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte27SourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte27SourceSettings\"\n          }\n        }\n      ]\n    },\n    \"TeletextSourceSettings\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TeletextSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"teletextSourceSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-selector-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CaptionSelectorSettings
---
