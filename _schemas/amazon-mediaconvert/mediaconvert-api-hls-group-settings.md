---
description: Settings related to your HLS output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to HLS_GROUP_SETTINGS.
layout: schema
name: HlsGroupSettings
properties_list:
- description: ''
  name: AdMarkers
  type: object
- description: ''
  name: AdditionalManifests
  type: object
- description: ''
  name: AudioOnlyHeader
  type: object
- description: ''
  name: BaseUrl
  type: object
- description: ''
  name: CaptionLanguageMappings
  type: object
- description: ''
  name: CaptionLanguageSetting
  type: object
- description: ''
  name: CaptionSegmentLengthControl
  type: object
- description: ''
  name: ClientCache
  type: object
- description: ''
  name: CodecSpecification
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: DestinationSettings
  type: object
- description: ''
  name: DirectoryStructure
  type: object
- description: ''
  name: Encryption
  type: object
- description: ''
  name: ImageBasedTrickPlay
  type: object
- description: ''
  name: ImageBasedTrickPlaySettings
  type: object
- description: ''
  name: ManifestCompression
  type: object
- description: ''
  name: ManifestDurationFormat
  type: object
- description: ''
  name: MinFinalSegmentLength
  type: object
- description: ''
  name: MinSegmentLength
  type: object
- description: ''
  name: OutputSelection
  type: object
- description: ''
  name: ProgramDateTime
  type: object
- description: ''
  name: ProgramDateTimePeriod
  type: object
- description: ''
  name: SegmentControl
  type: object
- description: ''
  name: SegmentLength
  type: object
- description: ''
  name: SegmentLengthControl
  type: object
- description: ''
  name: SegmentsPerSubdirectory
  type: object
- description: ''
  name: StreamInfResolution
  type: object
- description: ''
  name: TargetDurationCompatibilityMode
  type: object
- description: ''
  name: TimedMetadataId3Frame
  type: object
- description: ''
  name: TimedMetadataId3Period
  type: object
- description: ''
  name: TimestampDeltaMilliseconds
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-group-settings-schema.json
slug: mediaconvert-api-hls-group-settings
source_filename: mediaconvert-api-hls-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-group-settings-schema.json\",\n  \"title\": \"HlsGroupSettings\",\n  \"description\": \"Settings related to your HLS output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to HLS_GROUP_SETTINGS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdMarkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHlsAdMarkers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adMarkers\"\n          },\n          \"description\": \"Choose one or more ad marker types to decorate your Apple HLS manifest. This setting does\
  \ not determine whether SCTE-35 markers appear in the outputs themselves.\"\n        }\n      ]\n    },\n    \"AdditionalManifests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHlsAdditionalManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"additionalManifests\"\n          },\n          \"description\": \"By default, the service creates one top-level .m3u8 HLS manifest for each HLS output group in your job. This default manifest references every output in the output group. To create additional top-level manifests that reference a subset of the outputs in the output group, specify a list of them here.\"\n        }\n      ]\n    },\n    \"AudioOnlyHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsAudioOnlyHeader\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioOnlyHeader\"\n          },\n          \"description\": \"Ignore this setting unless you are\
  \ using FairPlay DRM with Verimatrix and you encounter playback issues. Keep the default value, Include (INCLUDE), to output audio-only headers. Choose Exclude (EXCLUDE) to remove the audio-only headers from your audio segments.\"\n        }\n      ]\n    },\n    \"BaseUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"baseUrl\"\n          },\n          \"description\": \"A partial URI prefix that will be prepended to each output in the media .m3u8 file. Can be used if base manifest is delivered from a different URL than the main .m3u8 file.\"\n        }\n      ]\n    },\n    \"CaptionLanguageMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHlsCaptionLanguageMapping\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionLanguageMappings\"\n          },\n          \"description\": \"Language to be used on\
  \ Caption outputs\"\n        }\n      ]\n    },\n    \"CaptionLanguageSetting\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsCaptionLanguageSetting\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionLanguageSetting\"\n          },\n          \"description\": \"Applies only to 608 Embedded output captions. Insert: Include CLOSED-CAPTIONS lines in the manifest. Specify at least one language in the CC1 Language Code field. One CLOSED-CAPTION line is added for each Language Code you specify. Make sure to specify the languages in the order in which they appear in the original source (if the source is embedded format) or the order of the caption selectors (if the source is other than embedded). Otherwise, languages in the manifest will not match up properly with the output captions. None: Include CLOSED-CAPTIONS=NONE line in the manifest. Omit: Omit any CLOSED-CAPTIONS line from the manifest.\"\n        }\n      ]\n    },\n    \"\
  CaptionSegmentLengthControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsCaptionSegmentLengthControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionSegmentLengthControl\"\n          },\n          \"description\": \"Set Caption segment length control (CaptionSegmentLengthControl) to Match video (MATCH_VIDEO) to create caption segments that align with the video segments from the first video output in this output group. For example, if the video segments are 2 seconds long, your WebVTT segments will also be 2 seconds long. Keep the default setting, Large segments (LARGE_SEGMENTS) to create caption segments that are 300 seconds long.\"\n        }\n      ]\n    },\n    \"ClientCache\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsClientCache\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientCache\"\n          },\n          \"description\": \"Disable this setting\
  \ only when your workflow requires the #EXT-X-ALLOW-CACHE:no tag. Otherwise, keep the default value Enabled (ENABLED) and control caching in your video distribution set up. For example, use the Cache-Control http header.\"\n        }\n      ]\n    },\n    \"CodecSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsCodecSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecSpecification\"\n          },\n          \"description\": \"Specification to use (RFC-6381 or the default RFC-4281) during m3u8 playlist generation.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"Use Destination (Destination) to specify the S3 output location and the output filename base. Destination accepts format\
  \ identifiers. If you do not specify the base filename in the URI, the service will use the filename of the input file. If your job has multiple inputs, the service uses the filename of the first input file.\"\n        }\n      ]\n    },\n    \"DestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationSettings\"\n          },\n          \"description\": \"Settings associated with the destination. Will vary based on the type of destination\"\n        }\n      ]\n    },\n    \"DirectoryStructure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsDirectoryStructure\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"directoryStructure\"\n          },\n          \"description\": \"Indicates whether segments should be placed in subdirectories.\"\n        }\n      ]\n    },\n    \"Encryption\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsEncryptionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          },\n          \"description\": \"DRM settings.\"\n        }\n      ]\n    },\n    \"ImageBasedTrickPlay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsImageBasedTrickPlay\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageBasedTrickPlay\"\n          },\n          \"description\": \"Specify whether MediaConvert generates images for trick play. Keep the default value, None (NONE), to not generate any images. Choose Thumbnail (THUMBNAIL) to generate tiled thumbnails. Choose Thumbnail and full frame (THUMBNAIL_AND_FULLFRAME) to generate tiled thumbnails and full-resolution images of single frames. MediaConvert creates a child manifest for each set of images that you generate and adds corresponding entries to the parent manifest. A common application\
  \ for these images is Roku trick mode. The thumbnails and full-frame images that MediaConvert creates with this feature are compatible with this Roku specification: https://developer.roku.com/docs/developer-program/media-playback/trick-mode/hls-and-dash.md\"\n        }\n      ]\n    },\n    \"ImageBasedTrickPlaySettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsImageBasedTrickPlaySettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageBasedTrickPlaySettings\"\n          },\n          \"description\": \"Tile and thumbnail settings applicable when imageBasedTrickPlay is ADVANCED\"\n        }\n      ]\n    },\n    \"ManifestCompression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsManifestCompression\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestCompression\"\n          },\n          \"description\": \"When set to GZIP, compresses HLS playlist.\"\n\
  \        }\n      ]\n    },\n    \"ManifestDurationFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsManifestDurationFormat\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestDurationFormat\"\n          },\n          \"description\": \"Indicates whether the output manifest should use floating point values for segment duration.\"\n        }\n      ]\n    },\n    \"MinFinalSegmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minFinalSegmentLength\"\n          },\n          \"description\": \"Keep this setting at the default value of 0, unless you are troubleshooting a problem with how devices play back the end of your video asset. If you know that player devices are hanging on the final segment of your video because the length of your final segment is too short, use this setting to specify\
  \ a minimum final segment length, in seconds. Choose a value that is greater than or equal to 1 and less than your segment length. When you specify a value for this setting, the encoder will combine any final segment that is shorter than the length that you specify with the previous segment. For example, your segment length is 3 seconds and your final segment is .5 seconds without a minimum final segment length; when you set the minimum final segment length to 1, your final segment is 3.5 seconds.\"\n        }\n      ]\n    },\n    \"MinSegmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minSegmentLength\"\n          },\n          \"description\": \"When set, Minimum Segment Size is enforced by looking ahead and back within the specified range for a nearby avail and extending the segment size if needed.\"\n        }\n      ]\n    },\n    \"OutputSelection\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsOutputSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputSelection\"\n          },\n          \"description\": \"Indicates whether the .m3u8 manifest file should be generated for this HLS output group.\"\n        }\n      ]\n    },\n    \"ProgramDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsProgramDateTime\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programDateTime\"\n          },\n          \"description\": \"Includes or excludes EXT-X-PROGRAM-DATE-TIME tag in .m3u8 manifest files. The value is calculated as follows: either the program date and time are initialized using the input timecode source, or the time is initialized using the input timecode source and the date is initialized using the timestamp_offset.\"\n        }\n      ]\n    },\n    \"ProgramDateTimePeriod\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max3600\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programDateTimePeriod\"\n          },\n          \"description\": \"Period of insertion of EXT-X-PROGRAM-DATE-TIME entry, in seconds.\"\n        }\n      ]\n    },\n    \"SegmentControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsSegmentControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentControl\"\n          },\n          \"description\": \"When set to SINGLE_FILE, emits program as a single media resource (.ts) file, uses #EXT-X-BYTERANGE tags to index segment for playback.\"\n        }\n      ]\n    },\n    \"SegmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentLength\"\n          },\n          \"description\": \"Specify the\
  \ length, in whole seconds, of each segment. When you don't specify a value, MediaConvert defaults to 10. Related settings: Use Segment length control (SegmentLengthControl) to specify whether the encoder enforces this value strictly. Use Segment control (HlsSegmentControl) to specify whether MediaConvert creates separate segment files or one content file that has metadata to mark the segment boundaries.\"\n        }\n      ]\n    },\n    \"SegmentLengthControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsSegmentLengthControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentLengthControl\"\n          },\n          \"description\": \"Specify how you want MediaConvert to determine the segment length. Choose Exact (EXACT) to have the encoder use the exact length that you specify with the setting Segment length (SegmentLength). This might result in extra I-frames. Choose Multiple of GOP (GOP_MULTIPLE) to have the encoder round\
  \ up the segment lengths to match the next GOP boundary.\"\n        }\n      ]\n    },\n    \"SegmentsPerSubdirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentsPerSubdirectory\"\n          },\n          \"description\": \"Number of segments to write to a subdirectory before starting a new one. directoryStructure must be SINGLE_DIRECTORY for this setting to have an effect.\"\n        }\n      ]\n    },\n    \"StreamInfResolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsStreamInfResolution\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamInfResolution\"\n          },\n          \"description\": \"Include or exclude RESOLUTION attribute for video in EXT-X-STREAM-INF tag of variant manifest.\"\n        }\n      ]\n    },\n    \"TargetDurationCompatibilityMode\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/HlsTargetDurationCompatibilityMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetDurationCompatibilityMode\"\n          },\n          \"description\": \"When set to LEGACY, the segment target duration is always rounded up to the nearest integer value above its current value in seconds. When set to SPEC\\\\\\\\_COMPLIANT, the segment target duration is rounded up to the nearest integer value if fraction seconds are greater than or equal to 0.5 (>= 0.5) and rounded down if less than 0.5 (< 0.5). You may need to use LEGACY if your client needs to ensure that the target duration is always longer than the actual duration of the segment. Some older players may experience interrupted playback when the actual duration of a track in a segment is longer than the target duration.\"\n        }\n      ]\n    },\n    \"TimedMetadataId3Frame\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsTimedMetadataId3Frame\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataId3Frame\"\n          },\n          \"description\": \"Specify the type of the ID3 frame (timedMetadataId3Frame) to use for ID3 timestamps (timedMetadataId3Period) in your output. To include ID3 timestamps: Specify PRIV (PRIV) or TDRL (TDRL) and set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH). To exclude ID3 timestamps: Set ID3 timestamp frame type to None (NONE).\"\n        }\n      ]\n    },\n    \"TimedMetadataId3Period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataId3Period\"\n          },\n          \"description\": \"Specify the interval in seconds to write ID3 timestamps in your output. The first timestamp starts at the output timecode and date, and increases incrementally with each ID3 timestamp. To use the default interval\
  \ of 10 seconds: Leave blank. To include this metadata in your output: Set ID3 timestamp frame type (timedMetadataId3Frame) to PRIV (PRIV) or TDRL (TDRL), and set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH).\"\n        }\n      ]\n    },\n    \"TimestampDeltaMilliseconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timestampDeltaMilliseconds\"\n          },\n          \"description\": \"Provides an extra millisecond delta offset to fine tune the timestamps.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-group-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsGroupSettings
---
