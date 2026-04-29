---
description: Hls Group Settings
layout: schema
name: HlsGroupSettings
properties_list:
- description: ''
  name: AdMarkers
  type: object
- description: ''
  name: BaseUrlContent
  type: object
- description: ''
  name: BaseUrlContent1
  type: object
- description: ''
  name: BaseUrlManifest
  type: object
- description: ''
  name: BaseUrlManifest1
  type: object
- description: ''
  name: CaptionLanguageMappings
  type: object
- description: ''
  name: CaptionLanguageSetting
  type: object
- description: ''
  name: ClientCache
  type: object
- description: ''
  name: CodecSpecification
  type: object
- description: ''
  name: ConstantIv
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: DirectoryStructure
  type: object
- description: ''
  name: DiscontinuityTags
  type: object
- description: ''
  name: EncryptionType
  type: object
- description: ''
  name: HlsCdnSettings
  type: object
- description: ''
  name: HlsId3SegmentTagging
  type: object
- description: ''
  name: IFrameOnlyPlaylists
  type: object
- description: ''
  name: IncompleteSegmentBehavior
  type: object
- description: ''
  name: IndexNSegments
  type: object
- description: ''
  name: InputLossAction
  type: object
- description: ''
  name: IvInManifest
  type: object
- description: ''
  name: IvSource
  type: object
- description: ''
  name: KeepSegments
  type: object
- description: ''
  name: KeyFormat
  type: object
- description: ''
  name: KeyFormatVersions
  type: object
- description: ''
  name: KeyProviderSettings
  type: object
- description: ''
  name: ManifestCompression
  type: object
- description: ''
  name: ManifestDurationFormat
  type: object
- description: ''
  name: MinSegmentLength
  type: object
- description: ''
  name: Mode
  type: object
- description: ''
  name: OutputSelection
  type: object
- description: ''
  name: ProgramDateTime
  type: object
- description: ''
  name: ProgramDateTimeClock
  type: object
- description: ''
  name: ProgramDateTimePeriod
  type: object
- description: ''
  name: RedundantManifest
  type: object
- description: ''
  name: SegmentLength
  type: object
- description: ''
  name: SegmentationMode
  type: object
- description: ''
  name: SegmentsPerSubdirectory
  type: object
- description: ''
  name: StreamInfResolution
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
- description: ''
  name: TsFileMode
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-hls-group-settings-schema.json
slug: medialive-api-hls-group-settings
source_filename: medialive-api-hls-group-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-group-settings-schema.json\",\n  \"title\": \"HlsGroupSettings\",\n  \"description\": \"Hls Group Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdMarkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHlsAdMarkers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adMarkers\"\n          },\n          \"description\": \"Choose one or more ad marker types to pass SCTE35 signals through to this group of Apple HLS outputs.\"\n        }\n      ]\n    },\n    \"BaseUrlContent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"baseUrlContent\"\n          },\n          \"description\": \"A partial URI prefix\
  \ that will be prepended to each output in the media .m3u8 file. Can be used if base manifest is delivered from a different URL than the main .m3u8 file.\"\n        }\n      ]\n    },\n    \"BaseUrlContent1\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"baseUrlContent1\"\n          },\n          \"description\": \"Optional. One value per output group.\\n\\nThis field is required only if you are completing Base URL content A, and the downstream system has notified you that the media files for pipeline 1 of all outputs are in a location different from the media files for pipeline 0.\"\n        }\n      ]\n    },\n    \"BaseUrlManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"baseUrlManifest\"\n          },\n          \"description\": \"A partial URI prefix that\
  \ will be prepended to each output in the media .m3u8 file. Can be used if base manifest is delivered from a different URL than the main .m3u8 file.\"\n        }\n      ]\n    },\n    \"BaseUrlManifest1\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"baseUrlManifest1\"\n          },\n          \"description\": \"Optional. One value per output group.\\n\\nComplete this field only if you are completing Base URL manifest A, and the downstream system has notified you that the child manifest files for pipeline 1 of all outputs are in a location different from the child manifest files for pipeline 0.\"\n        }\n      ]\n    },\n    \"CaptionLanguageMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCaptionLanguageMapping\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionLanguageMappings\"\n          },\n\
  \          \"description\": \"Mapping of up to 4 caption channels to caption languages.  Is only meaningful if captionLanguageSetting is set to \\\"insert\\\".\"\n        }\n      ]\n    },\n    \"CaptionLanguageSetting\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsCaptionLanguageSetting\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionLanguageSetting\"\n          },\n          \"description\": \"Applies only to 608 Embedded output captions.\\ninsert: Include CLOSED-CAPTIONS lines in the manifest. Specify at least one language in the CC1 Language Code field. One CLOSED-CAPTION line is added for each Language Code you specify. Make sure to specify the languages in the order in which they appear in the original source (if the source is embedded format) or the order of the caption selectors (if the source is other than embedded). Otherwise, languages in the manifest will not match up properly with the output captions.\\nnone:\
  \ Include CLOSED-CAPTIONS=NONE line in the manifest.\\nomit: Omit any CLOSED-CAPTIONS line from the manifest.\"\n        }\n      ]\n    },\n    \"ClientCache\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsClientCache\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientCache\"\n          },\n          \"description\": \"When set to \\\"disabled\\\", sets the #EXT-X-ALLOW-CACHE:no tag in the manifest, which prevents clients from saving media segments for later replay.\"\n        }\n      ]\n    },\n    \"CodecSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsCodecSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecSpecification\"\n          },\n          \"description\": \"Specification to use (RFC-6381 or the default RFC-4281) during m3u8 playlist generation.\"\n        }\n      ]\n    },\n    \"ConstantIv\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/__stringMin32Max32\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"constantIv\"\n          },\n          \"description\": \"For use with encryptionType. This is a 128-bit, 16-byte hex value represented by a 32-character text string. If ivSource is set to \\\"explicit\\\" then this parameter is required and is used as the IV for encryption.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputLocationRef\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"A directory or HTTP destination for the HLS segments, manifest files, and encryption keys (if enabled).\"\n        }\n      ]\n    },\n    \"DirectoryStructure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsDirectoryStructure\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"directoryStructure\"\n          },\n          \"description\": \"Place segments in subdirectories.\"\n        }\n      ]\n    },\n    \"DiscontinuityTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsDiscontinuityTags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"discontinuityTags\"\n          },\n          \"description\": \"Specifies whether to insert EXT-X-DISCONTINUITY tags in the HLS child manifests for this output group.\\nTypically, choose Insert because these tags are required in the manifest (according to the HLS specification) and serve an important purpose.\\nChoose Never Insert only if the downstream system is doing real-time failover (without using the MediaLive automatic failover feature) and only if that downstream system has advised you to exclude the tags.\"\n        }\n      ]\n    },\n    \"EncryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsEncryptionType\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionType\"\n          },\n          \"description\": \"Encrypts the segments with the given encryption scheme.  Exclude this parameter if no encryption is desired.\"\n        }\n      ]\n    },\n    \"HlsCdnSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsCdnSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsCdnSettings\"\n          },\n          \"description\": \"Parameters that control interactions with the CDN.\"\n        }\n      ]\n    },\n    \"HlsId3SegmentTagging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsId3SegmentTaggingState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsId3SegmentTagging\"\n          },\n          \"description\": \"State of HLS ID3 Segment Tagging\"\n        }\n      ]\n    },\n    \"IFrameOnlyPlaylists\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/IFrameOnlyPlaylistType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"iFrameOnlyPlaylists\"\n          },\n          \"description\": \"DISABLED: Do not create an I-frame-only manifest, but do create the master and media manifests (according to the Output Selection field).\\n\\nSTANDARD: Create an I-frame-only manifest for each output that contains video, as well as the other manifests (according to the Output Selection field). The I-frame manifest contains a #EXT-X-I-FRAMES-ONLY tag to indicate it is I-frame only, and one or more #EXT-X-BYTERANGE entries identifying the I-frame position. For example, #EXT-X-BYTERANGE:160364@1461888\\\"\"\n        }\n      ]\n    },\n    \"IncompleteSegmentBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsIncompleteSegmentBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"incompleteSegmentBehavior\"\n          },\n\
  \          \"description\": \"Specifies whether to include the final (incomplete) segment in the media output when the pipeline stops producing output because of a channel stop, a channel pause or a loss of input to the pipeline.\\nAuto means that MediaLive decides whether to include the final segment, depending on the channel class and the types of output groups.\\nSuppress means to never include the incomplete segment. We recommend you choose Auto and let MediaLive control the behavior.\"\n        }\n      ]\n    },\n    \"IndexNSegments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"indexNSegments\"\n          },\n          \"description\": \"Applies only if Mode field is LIVE.\\n\\nSpecifies the maximum number of segments in the media manifest file. After this maximum, older segments are removed from the media manifest. This number must be smaller than the number in\
  \ the Keep Segments field.\"\n        }\n      ]\n    },\n    \"InputLossAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLossActionForHlsOut\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputLossAction\"\n          },\n          \"description\": \"Parameter that control output group behavior on input loss.\"\n        }\n      ]\n    },\n    \"IvInManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsIvInManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ivInManifest\"\n          },\n          \"description\": \"For use with encryptionType. The IV (Initialization Vector) is a 128-bit number used in conjunction with the key for encrypting blocks. If set to \\\"include\\\", IV is listed in the manifest, otherwise the IV is not in the manifest.\"\n        }\n      ]\n    },\n    \"IvSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsIvSource\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"ivSource\"\n          },\n          \"description\": \"For use with encryptionType. The IV (Initialization Vector) is a 128-bit number used in conjunction with the key for encrypting blocks. If this setting is \\\"followsSegmentNumber\\\", it will cause the IV to change every segment (to match the segment number). If this is set to \\\"explicit\\\", you must enter a constantIv value.\"\n        }\n      ]\n    },\n    \"KeepSegments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keepSegments\"\n          },\n          \"description\": \"Applies only if Mode field is LIVE.\\n\\nSpecifies the number of media segments to retain in the destination directory. This number should be bigger than indexNSegments (Num segments). We recommend (value = (2 x indexNsegments) + 1).\\n\\nIf this \\\"keep segments\\\"\
  \ number is too low, the following might happen: the player is still reading a media manifest file that lists this segment, but that segment has been removed from the destination directory (as directed by indexNSegments). This situation would result in a 404 HTTP error on the player.\"\n        }\n      ]\n    },\n    \"KeyFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyFormat\"\n          },\n          \"description\": \"The value specifies how the key is represented in the resource identified by the URI.  If parameter is absent, an implicit value of \\\"identity\\\" is used.  A reverse DNS string can also be given.\"\n        }\n      ]\n    },\n    \"KeyFormatVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyFormatVersions\"\n          },\n\
  \          \"description\": \"Either a single positive integer version value or a slash delimited list of version values (1/2/3).\"\n        }\n      ]\n    },\n    \"KeyProviderSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyProviderSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"keyProviderSettings\"\n          },\n          \"description\": \"The key provider settings.\"\n        }\n      ]\n    },\n    \"ManifestCompression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsManifestCompression\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestCompression\"\n          },\n          \"description\": \"When set to gzip, compresses HLS playlist.\"\n        }\n      ]\n    },\n    \"ManifestDurationFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsManifestDurationFormat\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"manifestDurationFormat\"\n          },\n          \"description\": \"Indicates whether the output manifest should use floating point or integer values for segment duration.\"\n        }\n      ]\n    },\n    \"MinSegmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minSegmentLength\"\n          },\n          \"description\": \"Minimum length of MPEG-2 Transport Stream segments in seconds. When set, minimum segment length is enforced by looking ahead and back within the specified range for a nearby avail and extending the segment size if needed.\"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mode\"\n          },\n          \"description\": \"If \\\"vod\\\", all segments are indexed\
  \ and kept permanently in the destination and manifest. If \\\"live\\\", only the number segments specified in keepSegments and indexNSegments are kept; newer segments replace older segments, which may prevent players from rewinding all the way to the beginning of the event.\\n\\nVOD mode uses HLS EXT-X-PLAYLIST-TYPE of EVENT while the channel is running, converting it to a \\\"VOD\\\" type manifest on completion of the stream.\"\n        }\n      ]\n    },\n    \"OutputSelection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsOutputSelection\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputSelection\"\n          },\n          \"description\": \"MANIFESTS_AND_SEGMENTS: Generates manifests (master manifest, if applicable, and media manifests) for this output group.\\n\\nVARIANT_MANIFESTS_AND_SEGMENTS: Generates media manifests for this output group, but not a master manifest.\\n\\nSEGMENTS_ONLY: Does not generate any manifests\
  \ for this output group.\"\n        }\n      ]\n    },\n    \"ProgramDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsProgramDateTime\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programDateTime\"\n          },\n          \"description\": \"Includes or excludes EXT-X-PROGRAM-DATE-TIME tag in .m3u8 manifest files. The value is calculated using the program date time clock.\"\n        }\n      ]\n    },\n    \"ProgramDateTimeClock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsProgramDateTimeClock\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programDateTimeClock\"\n          },\n          \"description\": \"Specifies the algorithm used to drive the HLS EXT-X-PROGRAM-DATE-TIME clock. Options include:\\n\\nINITIALIZE_FROM_OUTPUT_TIMECODE: The PDT clock is initialized as a function of the first output timecode, then incremented by the EXTINF duration of each encoded\
  \ segment.\\n\\nSYSTEM_CLOCK: The PDT clock is initialized as a function of the UTC wall clock, then incremented by the EXTINF duration of each encoded segment. If the PDT clock diverges from the wall clock by more than 500ms, it is resynchronized to the wall clock.\"\n        }\n      ]\n    },\n    \"ProgramDateTimePeriod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max3600\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programDateTimePeriod\"\n          },\n          \"description\": \"Period of insertion of EXT-X-PROGRAM-DATE-TIME entry, in seconds.\"\n        }\n      ]\n    },\n    \"RedundantManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsRedundantManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"redundantManifest\"\n          },\n          \"description\": \"ENABLED: The master manifest (.m3u8 file) for each pipeline includes information\
  \ about both pipelines: first its own media files, then the media files of the other pipeline. This feature allows playout device that support stale manifest detection to switch from one manifest to the other, when the current manifest seems to be stale. There are still two destinations and two master manifests, but both master manifests reference the media files from both pipelines.\\n\\nDISABLED: The master manifest (.m3u8 file) for each pipeline includes information about its own pipeline only.\\n\\nFor an HLS output group with MediaPackage as the destination, the DISABLED behavior is always followed. MediaPackage regenerates the manifests it serves to players so a redundant manifest from MediaLive is irrelevant.\"\n        }\n      ]\n    },\n    \"SegmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentLength\"\n          },\n          \"description\"\
  : \"Length of MPEG-2 Transport Stream segments to create in seconds. Note that segments will end on the next keyframe after this duration, so actual segment length may be longer.\"\n        }\n      ]\n    },\n    \"SegmentationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsSegmentationMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationMode\"\n          },\n          \"description\": \"useInputSegmentation has been deprecated. The configured segment size is always used.\"\n        }\n      ]\n    },\n    \"SegmentsPerSubdirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentsPerSubdirectory\"\n          },\n          \"description\": \"Number of segments to write to a subdirectory before starting a new one. directoryStructure must be subdirectoryPerStream for this setting to have an\
  \ effect.\"\n        }\n      ]\n    },\n    \"StreamInfResolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsStreamInfResolution\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamInfResolution\"\n          },\n          \"description\": \"Include or exclude RESOLUTION attribute for video in EXT-X-STREAM-INF tag of variant manifest.\"\n        }\n      ]\n    },\n    \"TimedMetadataId3Frame\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsTimedMetadataId3Frame\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataId3Frame\"\n          },\n          \"description\": \"Indicates ID3 frame that has the timecode.\"\n        }\n      ]\n    },\n    \"TimedMetadataId3Period\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataId3Period\"\
  \n          },\n          \"description\": \"Timed Metadata interval in seconds.\"\n        }\n      ]\n    },\n    \"TimestampDeltaMilliseconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timestampDeltaMilliseconds\"\n          },\n          \"description\": \"Provides an extra millisecond delta offset to fine tune the timestamps.\"\n        }\n      ]\n    },\n    \"TsFileMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsTsFileMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tsFileMode\"\n          },\n          \"description\": \"SEGMENTED_FILES: Emit the program as segments - multiple .ts media files.\\n\\nSINGLE_FILE: Applies only if Mode field is VOD. Emit the program as a single .ts media file. The media manifest includes #EXT-X-BYTERANGE tags to index segments for playback. A typical use for this\
  \ value is when sending the output to AWS Elemental MediaConvert, which can accept only a single media file. Playback while the channel is running is not guaranteed due to HTTP server caching.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-hls-group-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsGroupSettings
---
