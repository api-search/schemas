---
description: Settings related to your CMAF output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to CMAF_GROUP_SETTINGS.
layout: schema
name: CmafGroupSettings
properties_list:
- description: ''
  name: AdditionalManifests
  type: object
- description: ''
  name: BaseUrl
  type: object
- description: ''
  name: ClientCache
  type: object
- description: ''
  name: CodecSpecification
  type: object
- description: ''
  name: DashManifestStyle
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
  name: MinBufferTime
  type: object
- description: ''
  name: MinFinalSegmentLength
  type: object
- description: ''
  name: MpdManifestBandwidthType
  type: object
- description: ''
  name: MpdProfile
  type: object
- description: ''
  name: PtsOffsetHandlingForBFrames
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
  name: StreamInfResolution
  type: object
- description: ''
  name: TargetDurationCompatibilityMode
  type: object
- description: ''
  name: VideoCompositionOffsets
  type: object
- description: ''
  name: WriteDashManifest
  type: object
- description: ''
  name: WriteHlsManifest
  type: object
- description: ''
  name: WriteSegmentTimelineInRepresentation
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmaf-group-settings-schema.json
slug: mediaconvert-api-cmaf-group-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-group-settings-schema.json\",\n  \"title\": \"CmafGroupSettings\",\n  \"description\": \"Settings related to your CMAF output package. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/outputs-file-ABR.html. When you work directly in your JSON job specification, include this object and any required children when you set Type, under OutputGroupSettings, to CMAF_GROUP_SETTINGS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdditionalManifests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCmafAdditionalManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"additionalManifests\"\n          },\n          \"description\": \"By default, the service creates one top-level .m3u8 HLS\
  \ manifest and one top -level .mpd DASH manifest for each CMAF output group in your job. These default manifests reference every output in the output group. To create additional top-level manifests that reference a subset of the outputs in the output group, specify a list of them here. For each additional manifest that you specify, the service creates one HLS manifest and one DASH manifest.\"\n        }\n      ]\n    },\n    \"BaseUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"baseUrl\"\n          },\n          \"description\": \"A partial URI prefix that will be put in the manifest file at the top level BaseURL element. Can be used if streams are delivered from a different URL than the manifest file.\"\n        }\n      ]\n    },\n    \"ClientCache\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafClientCache\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"clientCache\"\n          },\n          \"description\": \"Disable this setting only when your workflow requires the #EXT-X-ALLOW-CACHE:no tag. Otherwise, keep the default value Enabled (ENABLED) and control caching in your video distribution set up. For example, use the Cache-Control http header.\"\n        }\n      ]\n    },\n    \"CodecSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafCodecSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecSpecification\"\n          },\n          \"description\": \"Specification to use (RFC-6381 or the default RFC-4281) during m3u8 playlist generation.\"\n        }\n      ]\n    },\n    \"DashManifestStyle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DashManifestStyle\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dashManifestStyle\"\n          },\n         \
  \ \"description\": \"Specify how MediaConvert writes SegmentTimeline in your output DASH manifest. To write a SegmentTimeline in each video Representation: Keep the default value, Basic. To write a common SegmentTimeline in the video AdaptationSet: Choose Compact. Note that MediaConvert will still write a SegmentTimeline in any Representation that does not share a common timeline. To write a video AdaptationSet for each different output framerate, and a common SegmentTimeline in each AdaptationSet: Choose Distinct.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"Use Destination (Destination) to specify the S3 output location and the output filename base. Destination accepts format identifiers. If you do not specify the base filename in the URI, the service will\
  \ use the filename of the input file. If your job has multiple inputs, the service uses the filename of the first input file.\"\n        }\n      ]\n    },\n    \"DestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationSettings\"\n          },\n          \"description\": \"Settings associated with the destination. Will vary based on the type of destination\"\n        }\n      ]\n    },\n    \"Encryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafEncryptionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryption\"\n          },\n          \"description\": \"DRM settings.\"\n        }\n      ]\n    },\n    \"FragmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"fragmentLength\"\n          },\n          \"description\": \"Specify the length, in whole seconds, of the mp4 fragments. When you don't specify a value, MediaConvert defaults to 2. Related setting: Use Fragment length control (FragmentLengthControl) to specify whether the encoder enforces this value strictly.\"\n        }\n      ]\n    },\n    \"ImageBasedTrickPlay\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafImageBasedTrickPlay\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageBasedTrickPlay\"\n          },\n          \"description\": \"Specify whether MediaConvert generates images for trick play. Keep the default value, None (NONE), to not generate any images. Choose Thumbnail (THUMBNAIL) to generate tiled thumbnails. Choose Thumbnail and full frame (THUMBNAIL_AND_FULLFRAME) to generate tiled thumbnails and full-resolution images of single frames. When you enable Write HLS manifest (WriteHlsManifest),\
  \ MediaConvert creates a child manifest for each set of images that you generate and adds corresponding entries to the parent manifest. When you enable Write DASH manifest (WriteDashManifest), MediaConvert adds an entry in the .mpd manifest for each set of images that you generate. A common application for these images is Roku trick mode. The thumbnails and full-frame images that MediaConvert creates with this feature are compatible with this Roku specification: https://developer.roku.com/docs/developer-program/media-playback/trick-mode/hls-and-dash.md\"\n        }\n      ]\n    },\n    \"ImageBasedTrickPlaySettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafImageBasedTrickPlaySettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageBasedTrickPlaySettings\"\n          },\n          \"description\": \"Tile and thumbnail settings applicable when imageBasedTrickPlay is ADVANCED\"\n        }\n      ]\n    },\n    \"ManifestCompression\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafManifestCompression\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestCompression\"\n          },\n          \"description\": \"When set to GZIP, compresses HLS playlist.\"\n        }\n      ]\n    },\n    \"ManifestDurationFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafManifestDurationFormat\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestDurationFormat\"\n          },\n          \"description\": \"Indicates whether the output manifest should use floating point values for segment duration.\"\n        }\n      ]\n    },\n    \"MinBufferTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minBufferTime\"\n          },\n          \"description\": \"Minimum time of initially\
  \ buffered media that is needed to ensure smooth playout.\"\n        }\n      ]\n    },\n    \"MinFinalSegmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minFinalSegmentLength\"\n          },\n          \"description\": \"Keep this setting at the default value of 0, unless you are troubleshooting a problem with how devices play back the end of your video asset. If you know that player devices are hanging on the final segment of your video because the length of your final segment is too short, use this setting to specify a minimum final segment length, in seconds. Choose a value that is greater than or equal to 1 and less than your segment length. When you specify a value for this setting, the encoder will combine any final segment that is shorter than the length that you specify with the previous segment. For example, your segment length is 3 seconds\
  \ and your final segment is .5 seconds without a minimum final segment length; when you set the minimum final segment length to 1, your final segment is 3.5 seconds.\"\n        }\n      ]\n    },\n    \"MpdManifestBandwidthType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafMpdManifestBandwidthType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mpdManifestBandwidthType\"\n          },\n          \"description\": \"Specify how the value for bandwidth is determined for each video Representation in your output MPD manifest. We recommend that you choose a MPD manifest bandwidth type that is compatible with your downstream player configuration. Max: Use the same value that you specify for Max bitrate in the video output, in bits per second. Average: Use the calculated average bitrate of the encoded video output, in bits per second.\"\n        }\n      ]\n    },\n    \"MpdProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/CmafMpdProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mpdProfile\"\n          },\n          \"description\": \"Specify whether your DASH profile is on-demand or main. When you choose Main profile (MAIN_PROFILE), the service signals urn:mpeg:dash:profile:isoff-main:2011 in your .mpd DASH manifest. When you choose On-demand (ON_DEMAND_PROFILE), the service signals urn:mpeg:dash:profile:isoff-on-demand:2011 in your .mpd. When you choose On-demand, you must also set the output group setting Segment control (SegmentControl) to Single file (SINGLE_FILE).\"\n        }\n      ]\n    },\n    \"PtsOffsetHandlingForBFrames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafPtsOffsetHandlingForBFrames\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ptsOffsetHandlingForBFrames\"\n          },\n          \"description\": \"Use this setting only when your output video stream has B-frames,\
  \ which causes the initial presentation time stamp (PTS) to be offset from the initial decode time stamp (DTS). Specify how MediaConvert handles PTS when writing time stamps in output DASH manifests. Choose Match initial PTS (MATCH_INITIAL_PTS) when you want MediaConvert to use the initial PTS as the first time stamp in the manifest. Choose Zero-based (ZERO_BASED) to have MediaConvert ignore the initial PTS in the video stream and instead write the initial time stamp as zero in the manifest. For outputs that don't have B-frames, the time stamps in your DASH manifests start at zero regardless of your choice here.\"\n        }\n      ]\n    },\n    \"SegmentControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafSegmentControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentControl\"\n          },\n          \"description\": \"When set to SINGLE_FILE, a single output file is generated, which is internally segmented using\
  \ the Fragment Length and Segment Length. When set to SEGMENTED_FILES, separate segment files will be created.\"\n        }\n      ]\n    },\n    \"SegmentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentLength\"\n          },\n          \"description\": \"Specify the length, in whole seconds, of each segment. When you don't specify a value, MediaConvert defaults to 10. Related settings: Use Segment length control (SegmentLengthControl) to specify whether the encoder enforces this value strictly. Use Segment control (CmafSegmentControl) to specify whether MediaConvert creates separate segment files or one content file that has metadata to mark the segment boundaries.\"\n        }\n      ]\n    },\n    \"SegmentLengthControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafSegmentLengthControl\"\n        },\n \
  \       {\n          \"xml\": {\n            \"name\": \"segmentLengthControl\"\n          },\n          \"description\": \"Specify how you want MediaConvert to determine the segment length. Choose Exact (EXACT) to have the encoder use the exact length that you specify with the setting Segment length (SegmentLength). This might result in extra I-frames. Choose Multiple of GOP (GOP_MULTIPLE) to have the encoder round up the segment lengths to match the next GOP boundary.\"\n        }\n      ]\n    },\n    \"StreamInfResolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafStreamInfResolution\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamInfResolution\"\n          },\n          \"description\": \"Include or exclude RESOLUTION attribute for video in EXT-X-STREAM-INF tag of variant manifest.\"\n        }\n      ]\n    },\n    \"TargetDurationCompatibilityMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafTargetDurationCompatibilityMode\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"targetDurationCompatibilityMode\"\n          },\n          \"description\": \"When set to LEGACY, the segment target duration is always rounded up to the nearest integer value above its current value in seconds. When set to SPEC\\\\\\\\_COMPLIANT, the segment target duration is rounded up to the nearest integer value if fraction seconds are greater than or equal to 0.5 (>= 0.5) and rounded down if less than 0.5 (< 0.5). You may need to use LEGACY if your client needs to ensure that the target duration is always longer than the actual duration of the segment. Some older players may experience interrupted playback when the actual duration of a track in a segment is longer than the target duration.\"\n        }\n      ]\n    },\n    \"VideoCompositionOffsets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafVideoCompositionOffsets\"\n        },\n        {\n          \"xml\": {\n      \
  \      \"name\": \"videoCompositionOffsets\"\n          },\n          \"description\": \"Specify the video sample composition time offset mode in the output fMP4 TRUN box. For wider player compatibility, set Video composition offsets to Unsigned or leave blank. The earliest presentation time may be greater than zero, and sample composition time offsets will increment using unsigned integers. For strict fMP4 video and audio timing, set Video composition offsets to Signed. The earliest presentation time will be equal to zero, and sample composition time offsets will increment using signed integers.\"\n        }\n      ]\n    },\n    \"WriteDashManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafWriteDASHManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"writeDashManifest\"\n          },\n          \"description\": \"When set to ENABLED, a DASH MPD manifest will be generated for this output.\"\n        }\n      ]\n   \
  \ },\n    \"WriteHlsManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafWriteHLSManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"writeHlsManifest\"\n          },\n          \"description\": \"When set to ENABLED, an Apple HLS manifest will be generated for this output.\"\n        }\n      ]\n    },\n    \"WriteSegmentTimelineInRepresentation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmafWriteSegmentTimelineInRepresentation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"writeSegmentTimelineInRepresentation\"\n          },\n          \"description\": \"When you enable Precise segment duration in DASH manifests (writeSegmentTimelineInRepresentation), your DASH manifest shows precise segment durations. The segment duration information appears inside the SegmentTimeline element, inside SegmentTemplate at the Representation level. When this feature isn't enabled,\
  \ the segment durations in your DASH manifest are approximate. The segment duration information appears in the duration attribute of the SegmentTemplate element.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-group-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CmafGroupSettings
---
