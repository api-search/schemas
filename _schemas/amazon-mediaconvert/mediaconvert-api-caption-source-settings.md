---
description: If your input captions are SCC, TTML, STL, SMI, SRT, or IMSC in an xml file, specify the URI of the input captions source file. If your input captions are IMSC in an IMF package, use TrackSourceSettings instead of FileSoureSettings.
layout: schema
name: CaptionSourceSettings
properties_list:
- description: ''
  name: AncillarySourceSettings
  type: object
- description: ''
  name: DvbSubSourceSettings
  type: object
- description: ''
  name: EmbeddedSourceSettings
  type: object
- description: ''
  name: FileSourceSettings
  type: object
- description: ''
  name: SourceType
  type: object
- description: ''
  name: TeletextSourceSettings
  type: object
- description: ''
  name: TrackSourceSettings
  type: object
- description: ''
  name: WebvttHlsSourceSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-caption-source-settings-schema.json
slug: mediaconvert-api-caption-source-settings
source_filename: mediaconvert-api-caption-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-source-settings-schema.json\",\n  \"title\": \"CaptionSourceSettings\",\n  \"description\": \"If your input captions are SCC, TTML, STL, SMI, SRT, or IMSC in an xml file, specify the URI of the input captions source file. If your input captions are IMSC in an IMF package, use TrackSourceSettings instead of FileSoureSettings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AncillarySourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AncillarySourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ancillarySourceSettings\"\n          },\n          \"description\": \"Settings for ancillary captions source.\"\n        }\n      ]\n    },\n    \"DvbSubSourceSettings\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/DvbSubSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSubSourceSettings\"\n          },\n          \"description\": \"DVB Sub Source Settings\"\n        }\n      ]\n    },\n    \"EmbeddedSourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmbeddedSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"embeddedSourceSettings\"\n          },\n          \"description\": \"Settings for embedded captions Source\"\n        }\n      ]\n    },\n    \"FileSourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fileSourceSettings\"\n          },\n          \"description\": \"If your input captions are SCC, SMI, SRT, STL, TTML, WebVTT, or IMSC 1.1 in an xml file, specify the URI of the input caption source\
  \ file. If your caption source is IMSC in an IMF package, use TrackSourceSettings instead of FileSoureSettings.\"\n        }\n      ]\n    },\n    \"SourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionSourceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceType\"\n          },\n          \"description\": \"Use Source (SourceType) to identify the format of your input captions. The service cannot auto-detect caption format.\"\n        }\n      ]\n    },\n    \"TeletextSourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TeletextSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"teletextSourceSettings\"\n          },\n          \"description\": \"Settings specific to Teletext caption sources, including Page number.\"\n        }\n      ]\n    },\n    \"TrackSourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrackSourceSettings\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"trackSourceSettings\"\n          },\n          \"description\": \"Settings specific to caption sources that are specified by track number. Currently, this is only IMSC captions in an IMF package. If your caption source is IMSC 1.1 in a separate xml file, use FileSourceSettings instead of TrackSourceSettings.\"\n        }\n      ]\n    },\n    \"WebvttHlsSourceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebvttHlsSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"webvttHlsSourceSettings\"\n          },\n          \"description\": \"Settings specific to WebVTT sources in HLS alternative rendition group. Specify the properties (renditionGroupId, renditionName or renditionLanguageCode) to identify the unique subtitle track among the alternative rendition groups present in the HLS manifest. If no unique track is found, or multiple tracks match\
  \ the specified properties, the job fails. If there is only one subtitle track in the rendition group, the settings can be left empty and the default subtitle track will be chosen. If your caption source is a sidecar file, use FileSourceSettings instead of WebvttHlsSourceSettings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-source-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CaptionSourceSettings
---
