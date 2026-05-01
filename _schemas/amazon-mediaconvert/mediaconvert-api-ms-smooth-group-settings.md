---
description: Settings related to your Microsoft Smooth Streaming output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to MS_SMOOTH_GROUP_SETTINGS.
layout: schema
name: MsSmoothGroupSettings
properties_list:
- description: ''
  name: AdditionalManifests
  type: object
- description: ''
  name: AudioDeduplication
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: DestinationSettings
  type: object
- description: ''
  name: Encryption
  type: object
- description: ''
  name: FragmentLength
  type: object
- description: ''
  name: FragmentLengthControl
  type: object
- description: ''
  name: ManifestEncoding
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-ms-smooth-group-settings-schema.json
slug: mediaconvert-api-ms-smooth-group-settings
source_filename: mediaconvert-api-ms-smooth-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ms-smooth-group-settings-schema.json\",\n  \"title\": \"MsSmoothGroupSettings\",\n  \"description\": \"Settings related to your Microsoft Smooth Streaming output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to MS_SMOOTH_GROUP_SETTINGS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdditionalManifests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMsSmoothAdditionalManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"additionalManifests\"\n          },\n          \"description\": \"By default, the\
  \ service creates one .ism Microsoft Smooth Streaming manifest for each Microsoft Smooth Streaming output group in your job. This default manifest references every output in the output group. To create additional manifests that reference a subset of the outputs in the output group, specify a list of them here.\"\n        }\n      ]\n    },\n    \"AudioDeduplication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MsSmoothAudioDeduplication\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDeduplication\"\n          },\n          \"description\": \"COMBINE_DUPLICATE_STREAMS combines identical audio encoding settings across a Microsoft Smooth output group into a single audio stream.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n   \
  \       \"description\": \"Use Destination (Destination) to specify the S3 output location and the output filename base. Destination accepts format identifiers. If you do not specify the base filename in the URI, the service will use the filename of the input file. If your job has multiple inputs, the service uses the filename of the first input file.\"\n        }\n      ]\n    },\n    \"DestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationSettings\"\n          },\n          \"description\": \"Settings associated with the destination. Will vary based on the type of destination\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MsSmoothEncryptionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          },\n          \"\
  description\": \"If you are using DRM, set DRM System (MsSmoothEncryptionSettings) to specify the value SpekeKeyProvider.\"\n        }\n      ]\n    },\n    \"FragmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fragmentLength\"\n          },\n          \"description\": \"Specify how you want MediaConvert to determine the fragment length. Choose Exact (EXACT) to have the encoder use the exact length that you specify with the setting Fragment length (FragmentLength). This might result in extra I-frames. Choose Multiple of GOP (GOP_MULTIPLE) to have the encoder round up the segment lengths to match the next GOP boundary.\"\n        }\n      ]\n    },\n    \"FragmentLengthControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MsSmoothFragmentLengthControl\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"fragmentLengthControl\"\n          },\n          \"description\": \"Specify how you want MediaConvert to determine the fragment length. Choose Exact (EXACT) to have the encoder use the exact length that you specify with the setting Fragment length (FragmentLength). This might result in extra I-frames. Choose Multiple of GOP (GOP_MULTIPLE) to have the encoder round up the segment lengths to match the next GOP boundary.\"\n        }\n      ]\n    },\n    \"ManifestEncoding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MsSmoothManifestEncoding\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestEncoding\"\n          },\n          \"description\": \"Use Manifest encoding (MsSmoothManifestEncoding) to specify the encoding format for the server and client manifest. Valid options are utf8 and utf16.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ms-smooth-group-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MsSmoothGroupSettings
---
