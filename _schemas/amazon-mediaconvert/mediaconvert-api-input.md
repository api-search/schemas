---
description: Use inputs to define the source files used in your transcoding job. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/specify-input-settings.html. You can use multiple video inputs to do input stitching. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/assembling-multiple-inputs-and-input-clips.html
layout: schema
name: Input
properties_list:
- description: ''
  name: AudioSelectorGroups
  type: object
- description: ''
  name: AudioSelectors
  type: object
- description: ''
  name: CaptionSelectors
  type: object
- description: ''
  name: Crop
  type: object
- description: ''
  name: DeblockFilter
  type: object
- description: ''
  name: DecryptionSettings
  type: object
- description: ''
  name: DenoiseFilter
  type: object
- description: ''
  name: DolbyVisionMetadataXml
  type: object
- description: ''
  name: FileInput
  type: object
- description: ''
  name: FilterEnable
  type: object
- description: ''
  name: FilterStrength
  type: object
- description: ''
  name: ImageInserter
  type: object
- description: ''
  name: InputClippings
  type: object
- description: ''
  name: InputScanType
  type: object
- description: ''
  name: Position
  type: object
- description: ''
  name: ProgramNumber
  type: object
- description: ''
  name: PsiControl
  type: object
- description: ''
  name: SupplementalImps
  type: object
- description: ''
  name: TimecodeSource
  type: object
- description: ''
  name: TimecodeStart
  type: object
- description: ''
  name: VideoGenerator
  type: object
- description: ''
  name: VideoSelector
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-input-schema.json
slug: mediaconvert-api-input
source_filename: mediaconvert-api-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-schema.json\",\n  \"title\": \"Input\",\n  \"description\": \"Use inputs to define the source files used in your transcoding job. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/specify-input-settings.html. You can use multiple video inputs to do input stitching. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/assembling-multiple-inputs-and-input-clips.html\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioSelectorGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOfAudioSelectorGroup\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioSelectorGroups\"\n          },\n          \"description\": \"Use audio selector groups to combine multiple sidecar\
  \ audio inputs so that you can assign them to a single output audio tab (AudioDescription). Note that, if you're working with embedded audio, it's simpler to assign multiple input tracks into a single audio selector rather than use an audio selector group.\"\n        }\n      ]\n    },\n    \"AudioSelectors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOfAudioSelector\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioSelectors\"\n          },\n          \"description\": \"Use Audio selectors (AudioSelectors) to specify a track or set of tracks from the input that you will use in your outputs. You can use multiple Audio selectors per input.\"\n        }\n      ]\n    },\n    \"CaptionSelectors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOfCaptionSelector\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionSelectors\"\n          },\n          \"description\"\
  : \"Use captions selectors to specify the captions data from your input that you use in your outputs. You can use up to 20 captions selectors per input.\"\n        }\n      ]\n    },\n    \"Crop\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rectangle\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"crop\"\n          },\n          \"description\": \"Use Cropping selection (crop) to specify the video area that the service will include in the output video frame. If you specify a value here, it will override any value that you specify in the output setting Cropping selection (crop).\"\n        }\n      ]\n    },\n    \"DeblockFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeblockFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deblockFilter\"\n          },\n          \"description\": \"Enable Deblock (InputDeblockFilter) to produce smoother motion in the output.\
  \ Default is disabled. Only manually controllable for MPEG2 and uncompressed video inputs.\"\n        }\n      ]\n    },\n    \"DecryptionSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDecryptionSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"decryptionSettings\"\n          },\n          \"description\": \"Settings for decrypting any input files that you encrypt before you upload them to Amazon S3. MediaConvert can decrypt files only when you use AWS Key Management Service (KMS) to encrypt the data key that you use to encrypt your content.\"\n        }\n      ]\n    },\n    \"DenoiseFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDenoiseFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"denoiseFilter\"\n          },\n          \"description\": \"Enable Denoise (InputDenoiseFilter) to filter noise from the input. Default is disabled. Only\
  \ applicable to MPEG2, H.264, H.265, and uncompressed video inputs.\"\n        }\n      ]\n    },\n    \"DolbyVisionMetadataXml\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin14PatternS3XmlXMLHttpsXmlXML\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dolbyVisionMetadataXml\"\n          },\n          \"description\": \"Use this setting only when your video source has Dolby Vision studio mastering metadata that is carried in a separate XML file. Specify the Amazon S3 location for the metadata XML file. MediaConvert uses this file to provide global and frame-level metadata for Dolby Vision preprocessing. When you specify a file here and your input also has interleaved global and frame level metadata, MediaConvert ignores the interleaved metadata and uses only the the metadata from this external XML file. Note that your IAM service role must grant MediaConvert read permissions to this file. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/iam-role.html.\"\
  \n        }\n      ]\n    },\n    \"FileInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3Https\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fileInput\"\n          },\n          \"description\": \"Specify the source file for your transcoding job. You can use multiple inputs in a single job. The service concatenates these inputs, in the order that you specify them in the job, to create the outputs. If your input format is IMF, specify your input by providing the path to your CPL. For example, \\\"s3://bucket/vf/cpl.xml\\\". If the CPL is in an incomplete IMP, make sure to use *Supplemental IMPs* (SupplementalImps) to specify any supplemental IMPs that contain assets referenced by the CPL.\"\n        }\n      ]\n    },\n    \"FilterEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputFilterEnable\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterEnable\"\
  \n          },\n          \"description\": \"Specify how the transcoding service applies the denoise and deblock filters. You must also enable the filters separately, with Denoise (InputDenoiseFilter) and Deblock (InputDeblockFilter). * Auto - The transcoding service determines whether to apply filtering, depending on input type and quality. * Disable - The input is not filtered. This is true even if you use the API to enable them in (InputDeblockFilter) and (InputDeblockFilter). * Force - The input is filtered regardless of input type.\"\n        }\n      ]\n    },\n    \"FilterStrength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max5\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterStrength\"\n          },\n          \"description\": \"Use Filter strength (FilterStrength) to adjust the magnitude the input filter settings (Deblock and Denoise). The range is 0 to 5. Default is 0.\"\n        }\n      ]\n    },\n\
  \    \"ImageInserter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageInserter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"imageInserter\"\n          },\n          \"description\": \"Enable the image inserter feature to include a graphic overlay on your video. Enable or disable this feature for each input individually. This setting is disabled by default.\"\n        }\n      ]\n    },\n    \"InputClippings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInputClipping\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputClippings\"\n          },\n          \"description\": \"(InputClippings) contains sets of start and end times that together specify a portion of the input to be used in the outputs. If you provide only a start time, the clip will be the entire input from that point to the end. If you provide only an end time, it will be the entire input up to that\
  \ point. When you specify more than one input clip, the transcoding service creates the job outputs by stringing the clips together in the order you specify them.\"\n        }\n      ]\n    },\n    \"InputScanType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputScanType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputScanType\"\n          },\n          \"description\": \"When you have a progressive segmented frame (PsF) input, use this setting to flag the input as PsF. MediaConvert doesn't automatically detect PsF. Therefore, flagging your input as PsF results in better preservation of video quality when you do deinterlacing and frame rate conversion. If you don't specify, the default value is Auto (AUTO). Auto is the correct setting for all inputs that are not PsF. Don't set this value to PsF when your input is interlaced. Doing so creates horizontal interlacing artifacts.\"\n        }\n      ]\n    },\n    \"Position\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rectangle\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"position\"\n          },\n          \"description\": \"Use Selection placement (position) to define the video area in your output frame. The area outside of the rectangle that you specify here is black. If you specify a value here, it will override any value that you specify in the output setting Selection placement (position). If you specify a value here, this will override any AFD values in your input, even if you set Respond to AFD (RespondToAfd) to Respond (RESPOND). If you specify a value here, this will ignore anything that you specify for the setting Scaling Behavior (scalingBehavior).\"\n        }\n      ]\n    },\n    \"ProgramNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programNumber\"\
  \n          },\n          \"description\": \"Use Program (programNumber) to select a specific program from within a multi-program transport stream. Note that Quad 4K is not currently supported. Default is the first program within the transport stream. If the program you specify doesn't exist, the transcoding service will use this default.\"\n        }\n      ]\n    },\n    \"PsiControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputPsiControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"psiControl\"\n          },\n          \"description\": \"Set PSI control (InputPsiControl) for transport stream inputs to specify which data the demux process to scans. * Ignore PSI - Scan all PIDs for audio and video. * Use PSI - Scan only PSI data.\"\n        }\n      ]\n    },\n    \"SupplementalImps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__stringPatternS3ASSETMAPXml\"\n        },\n     \
  \   {\n          \"xml\": {\n            \"name\": \"supplementalImps\"\n          },\n          \"description\": \"Provide a list of any necessary supplemental IMPs. You need supplemental IMPs if the CPL that you're using for your input is in an incomplete IMP. Specify either the supplemental IMP directories with a trailing slash or the ASSETMAP.xml files. For example [\\\"s3://bucket/ov/\\\", \\\"s3://bucket/vf2/ASSETMAP.xml\\\"]. You don't need to specify the IMP that contains your input CPL, because the service automatically detects it.\"\n        }\n      ]\n    },\n    \"TimecodeSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputTimecodeSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeSource\"\n          },\n          \"description\": \"Use this Timecode source setting, located under the input settings (InputTimecodeSource), to specify how the service counts input video frames. This input frame count affects\
  \ only the behavior of features that apply to a single input at a time, such as input clipping and synchronizing some captions formats. Choose Embedded (EMBEDDED) to use the timecodes in your input video. Choose Start at zero (ZEROBASED) to start the first frame at zero. Choose Specified start (SPECIFIEDSTART) to start the first frame at the timecode that you specify in the setting Start timecode (timecodeStart). If you don't specify a value for Timecode source, the service will use Embedded by default. For more information about timecodes, see https://docs.aws.amazon.com/console/mediaconvert/timecode.\"\n        }\n      ]\n    },\n    \"TimecodeStart\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin11Max11Pattern01D20305D205D\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeStart\"\n          },\n          \"description\": \"Specify the timecode that you want the service to use for this input's initial frame. To\
  \ use this setting, you must set the Timecode source setting, located under the input settings (InputTimecodeSource), to Specified start (SPECIFIEDSTART). For more information about timecodes, see https://docs.aws.amazon.com/console/mediaconvert/timecode.\"\n        }\n      ]\n    },\n    \"VideoGenerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputVideoGenerator\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoGenerator\"\n          },\n          \"description\": \"When you include Video generator, MediaConvert creates a video input with black frames. Use this setting if you do not have a video input or if you want to add black video frames before, or after, other inputs. You can specify Video generator, or you can specify an Input file, but you cannot specify both. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/video-generator.html\"\n        }\n      ]\n    },\n    \"VideoSelector\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoSelector\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoSelector\"\n          },\n          \"description\": \"Input video selectors contain the video settings for the input. Each of your inputs can have up to one video selector.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-input-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Input
---
